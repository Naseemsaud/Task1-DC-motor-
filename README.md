# Task1-2 DC motor system code: 
void setup()
{
  pinMode(3, OUTPUT);
  pinMode(5, OUTPUT);
  pinMode(10, OUTPUT);
  pinMode(11, OUTPUT);}
void forward(){
  digitalWrite(3, HIGH);
  digitalWrite(5, LOW);
  digitalWrite(10, LOW);
  digitalWrite(11, HIGH);
  delay(2000);}
void backward(){
  digitalWrite(3, 0);
  digitalWrite(5, 1);
  digitalWrite(10, 1);
  digitalWrite(11, 0);
  delay(2000);}
void stopmotor(){ 
  digitalWrite(3, 0);
  digitalWrite(5, 0);
  digitalWrite(10, 0);
  digitalWrite(11, 0);
  delay(2000);}
void loop(){
forward();
 stopmotor();
 backward();}

