# RCspeed

#include
<Servo.h> Servo RC;   
int a = 0;  
void setup() {  
RC.attach(9);   
pinMode(4,INPUT);  
}  
  
void loop() {  
if (digitalRead(4) == 0)   
{  
while(digitalRead(4) == 0);   
a = (a+1)%7; delay(250);  
}   
switch(a){  
case 0:   
RC.write(0);  
break;   
case 1:   
RC.write(30);  
break;  
case 2:  
RC.write(60);  
break;  
case 3:  
RC.write(90);  
break; case 4:  
RC.write(120);  
break;  
case 5:  
RC.write(150);   
break;  
case 6:  
RC.write(180);  
break;  
}  
}  
  
