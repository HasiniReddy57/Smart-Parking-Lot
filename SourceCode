#include<Wire.h> 
#include <LiquidCrystal_I2C.h> 
LiquidCrystal_I2C lcd(0x27,16,2); 
#include<Servo.h> 
Servo myservo; 
#define trig1 7 
#define echo1 8 
#define trig2 9 
#define echo2 10 
int slots = 1; 
int in=0; 
void setup() 
{ 
 lcd.init(); 
 lcd.setBacklight(1); 
 lcd.setCursor(0,0); 
 Serial.begin (9600); 
 myservo.attach(6); 
 myservo.write(0); 
 lcd.setCursor (0,0); 
 lcd.print("ThemeBasedproject"); 
 lcd.setCursor (0,1); 
 lcd.print("SmartParkingLot"); 
 delay (2000); 
 lcd.clear(); 
} 
long Distance(int trigger, int echo) 
{ 
 pinMode(trigger, OUTPUT); 
 digitalWrite(trigger, LOW); 
 delayMicroseconds(2); 
 digitalWrite(trigger, HIGH); 
 delayMicroseconds(10);
