// C++ code
//
int red= 8;
int yellow=9;
int green=10;
int trig=3;
int echo=5;
long time;
int dist;
int threshold=200;
void setup()
{
  pinMode(trig, OUTPUT);
  pinMode(red, OUTPUT);
  pinMode(yellow, OUTPUT);
  pinMode(green, OUTPUT);
  pinMode(echo, INPUT);
  Serial.begin(9600);
}
void loop()
{
  digitalWrite(trig, LOW);
  delayMicroseconds(2);
  digitalWrite(trig, HIGH);
  delayMicroseconds(2);
  digitalWrite(trig,LOW);
  time= pulseIn(echo,HIGH);
  dist= time*0.034/2;
  Serial.println(dist);
  if (dist>threshold)
  {digitalWrite(red,LOW);
  digitalWrite(yellow,LOW);
  digitalWrite(green,HIGH);
  }
  else
  {digitalWrite(red,LOW);
  digitalWrite(yellow,HIGH);
  digitalWrite(green,LOW);
  delay(2000);
  digitalWrite(red,HIGH);
  digitalWrite(yellow,LOW);
  digitalWrite(green,LOW);
  while (true) {
    digitalWrite(trig, LOW);
    delayMicroseconds(2);
    digitalWrite(trig, HIGH);
    delayMicroseconds(2);
    digitalWrite(trig, LOW);
    time = pulseIn(echo, HIGH);
    dist = time * 0.034 / 2;
    if (dist >threshold)
    {break;}

  }
   delay(500); 
  }}
