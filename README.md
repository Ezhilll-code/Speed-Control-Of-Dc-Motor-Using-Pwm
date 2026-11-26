# Speed-Control-Of-Dc-Motor-Using-Pwm
Speed Control Of Dc Motor Using Pwm

### PROGRAM:
~~~
int MPin = 9;   //motor pin
int Analog = A0;  // Analog Input
int Ainp = 0; // Read analog input, initialized to zero  
  
void setup()
{
  
  Serial.begin(9600);
  pinMode(MPin, OUTPUT);
  pinMode(Analog, INPUT);
}

void loop()
{

Ainp = analogRead(A0);

int Speed = map(Ainp, 0, 1024, 0, 255);
delay(100);
Serial.println(Speed);
analogWrite(MPin, Speed);  

}
~~~
### OUTPUT :
<img width="1171" height="718" alt="PHOTO-2026-11-26-10-01-43" src="https://github.com/user-attachments/assets/85a4ad80-901b-469a-8ac2-b173e4d711d7" />

### RESULT :
Thus the program has been successfully executed and the result is verified.
