# 1201
int x=0;
void setup() {
  // put your setup code here, to run once:
pinMode (2,OUTPUT);
pinMode (7,INPUT);
pinMode (8,INPUT);
}

void loop() {
  // put your main code here, to run repeatedly:
  if(digitalRead(7)==1){
digitalWrite(2,HIGH);
delay (200);

}
if(digitalRead(7)==0){
digitalWrite(2,LOW);
delay (200);
}
