# Arduino-arm
Hi! I'm not a pro in Arduino projects ,but i had started a project named robot arm
#include<servo.h> 
Servo myservo; 
int joystick_x=A0; 
int servox; 
void setup() 
{ Serial.print(9600);
myservo.attach(3); } 
void loop() 
{ servox=analogRead(joystick_x); 
servox=map(servox,0,500,0,90); 
myservo.write(servox);
}
