Arduino Code 

#include <AccelStepper.h> 

 

// User Parameters 

const float syringeDiameter = 10.0;    // Diameter of the syringe in mm 

float flowRate = 10.0;     // Desired flow rate in mL/min 

bool readFlowRate = true; // True if we want to read the potentiometer 

 

// Physical parameters 

const float leadScrewPitch = 2.0;      // Lead screw pitch in mm/revolution 

const int stepsPerRevolution = 200;   // Motor steps per full revolution 

const float stepPerMM = stepsPerRevolution / leadScrewPitch; 

 

// Dynamic values 

float volumePerStep = (PI * pow((syringeDiameter / 2), 2) * leadScrewPitch) / (stepPerMM * 1000); 

float stepsPerSecond = (flowRate / volumePerStep) / 60.0; 

 

// Pin Setup 

const int blue = 8;     

const int red = 6;       

const int green = 7; 

 

const int pushButton = 4;  // number of the push button pin 

const int stopSwitch = 5;  // number of the stop button pin 

const int clockwiseButton = 9; 

const int counterClockwiseButton = 10; 

const int potentiometer = A0; 

const int debounceDelay = 50; // Delay for debouncing 

const int maxSpeed = 1000; 

 

const int stepPin = 2; // default step 

const int directionPin = 3; // default direction 

 

// const int ms1 = 11; // microstepping pin 1 

// const int ms2 = 12; // microstepping pin 2 

// const int ms3 = 13; // microstepping pin 3 

 

// State 

int pushButtonState = 1; 

int stopSwitchState = 0; 

int counterclockwise = 1; 

int clockwise = 1; 

 

// debounce 

const int NUM_BINS = 5;  // Number of flow rate bins 

 

float flowRateBins[NUM_BINS] = {0.5, 1.0, 2.5, 5.0, 10.0};  // mL/min 

 

int lastPotValue = 0; 

unsigned long lastDebounceTime = 0; 

 

AccelStepper stepper(AccelStepper::DRIVER, stepPin, directionPin); 

 

void setup() { 

 // initialize LED pins 

 pinMode(red, OUTPUT); 

 pinMode(green, OUTPUT); 

 pinMode(blue, OUTPUT); 

 

 // initialize push & stop button 

 pinMode(pushButton, INPUT_PULLUP); 

 pinMode(stopSwitch, INPUT_PULLUP); 

 

 // initialize direction buttons 

 pinMode(clockwiseButton, INPUT_PULLUP); 

 pinMode(counterClockwiseButton, INPUT_PULLUP); 

  //potentiometer 

 pinMode(potentiometer, INPUT); 

  stepper.setPinsInverted(true, false); 

 stepper.setMaxSpeed(maxSpeed); 

 stepper.setSpeed(50); 

 

 // serial 

 Serial.begin(9600); 

 

 Serial.print("Initial Flow Rate: "); 

 Serial.print(flowRate); 

 Serial.println(" mL/min"); 

} 

 

void updateFlowRateFromPotentiometer() { 

 delay(10); 

 stepper.runSpeed(); 

 // Create 6 discrete bins 

 float flowRates[] = {1.0, 2.5, 5.0, 10.0}; 

  // Read values 

 int potValue = analogRead(potentiometer); 

 int binIndex = map(potValue, 0, 1023, 0, 3); 

  // Check if flow rate has changed 

 if (flowRate != flowRates[binIndex]) { 

   flowRate = flowRates[binIndex]; 

   

   // Recalculate steps per second 

   stepsPerSecond = (flowRate / volumePerStep) / 60.0; 

   

   // Output flow rate change to Serial monitor 

   Serial.print("Flow Rate: "); 

   Serial.print(flowRate); 

   Serial.println(" mL/min"); 

 } 

} 

 

 

void loop() { 

 // Read the state of button values 

 pushButtonState = digitalRead(pushButton); 

 stopSwitchState = digitalRead(stopSwitch); 

 counterclockwise = digitalRead(counterClockwiseButton); 

 clockwise = digitalRead(clockwiseButton); 

 

 // Read the potentiometer value and set the flow rate 

 if(readFlowRate) { 

   updateFlowRateFromPotentiometer(); 

 } 

 

 stepper.setSpeed(stepsPerSecond); 

 

 // kill switch; reached the end 

 if (stopSwitchState == 0) { 

   digitalWrite(red, HIGH); 

   digitalWrite(green, LOW); 

   digitalWrite(blue, LOW); 

   stepper.setSpeed(0); 

 

 } 

 // if we're going 

 else if (pushButtonState == 0) { 

   digitalWrite(green, HIGH); 

   digitalWrite(blue, LOW); 

   digitalWrite(red, LOW); 

 

   if(counterclockwise == 0) { 

     digitalWrite(blue, HIGH); 

     stepper.setSpeed(-1 * maxSpeed); 

   } else if(clockwise == 0) { 

     digitalWrite(blue, HIGH); 

     stepper.setSpeed(maxSpeed); 

   } 

   

   stepper.runSpeed(); 

 } 

 // if we're stopped but not at the end 

 else { 

   digitalWrite(green, HIGH); 

   digitalWrite(red, HIGH); 

   digitalWrite(blue, LOW); 

 } 

 }  

 

 
