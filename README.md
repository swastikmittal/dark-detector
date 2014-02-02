dark-detector
============
const int ledpin =13; //choose pin 13 for led
const int inppin =2; //choose 2  for analog input

void setup()
{
pinMode(ledpin,OUTPUT); //set ledpin as output
pinMode(inputpin,OUTPUT); //set inputpin as input
}
void loop()
{int val = analogRead(inputpin);//initialise val

if(val > 0) //ie circuit forward biased 
{digitalWrite(ledpin,HIGH);}

if(val < 0) //ie circuit reversed biased 
{digitalWrite(ledpin,LOW);}}
