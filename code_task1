// C++ code
//

int red= 3;
int green= 6;
int yellow=5;
int switc= 2;
int present=0 ;
void setup()
{pinMode(green, OUTPUT);
 pinMode(yellow, OUTPUT);
  pinMode(red, OUTPUT);
 pinMode(switc, INPUT);
 Serial.begin(9600);
}

void loop()
{
int sw=digitalRead(switc);
  if(sw==0)
  {digitalWrite(green,HIGH);}
  else if(sw==1)
 {  digitalWrite(yellow,HIGH);
    digitalWrite(red,LOW);
    digitalWrite(green,LOW);
    delay(2000);
    digitalWrite(red,HIGH);
    digitalWrite(yellow,LOW);
    digitalWrite(green,LOW);
 delay(10000);
 digitalWrite(red,LOW);}}
