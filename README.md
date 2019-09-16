//SMARTINNOVATIONS..
int sensorpin = A0;

void setup ()
{
  Serial.begin(9600);
  pinMode(sensorpin , INPUT);
  
}

void loop()
{
  int value = analogRead(sensorpin);
  Serial.print("pin A0: ");
  Serial.println(value);
  delay(500);
}
