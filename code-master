int motorDer = 5; 
int motorIzq = 6; 
int ldrDer = A0; 
int ldrIzq = A1;  
int ValLdrDer = 0; 
int ValLdrIzq = 0;
int sensorpir = 12;
int ledVerde3 = 8;
int ledVerde4 = 9;
int ledRojo2 = 10;
int ledRojo1 = 11;

void setup() { 
  pinMode(motorDer, OUTPUT); 
  pinMode(motorIzq, OUTPUT); 
  pinMode(sensorpir, INPUT);
  pinMode(ldrIzq, INPUT);
  pinMode(ldrDer, INPUT);
  pinMode(ledRojo1, OUTPUT);
  pinMode(ledRojo2, OUTPUT);
  pinMode(ledVerde3, OUTPUT);
  pinMode(ledVerde4, OUTPUT);
  Serial.begin(750);
}

void loop() {
  ValLdrDer = analogRead(ldrDer);
  ValLdrIzq = analogRead(ldrIzq); 

  Serial.println(ValLdrDer);
  Serial.println(ValLdrIzq);
  
  if(ValLdrDer > 750) {
    digitalWrite(motorIzq, HIGH);
    digitalWrite(8,HIGH);
    digitalWrite(9,HIGH);
    digitalWrite(10,LOW);
    digitalWrite(11,LOW);
  }
  
  else;{
    digitalWrite(motorIzq, LOW);
    digitalWrite(11,HIGH);
    digitalWrite(10,HIGH);
    digitalWrite(9,LOW);
    digitalWrite(8,LOW);
  }
  if(ValLdrIzq > 750){
    digitalWrite(motorDer, HIGH);
    digitalWrite(8,HIGH);
    digitalWrite(9,HIGH);
    digitalWrite(10,LOW);
    digitalWrite(11,LOW);
  }
  else;{
    digitalWrite(motorDer, LOW);
    digitalWrite(11,HIGH);
    digitalWrite(10,HIGH);
    digitalWrite(9,LOW);
    digitalWrite(8,LOW);
  }
  if(digitalRead(sensorpir)== HIGH){
    Serial.println("Detectar movimiento por el sensor PIR");
    digitalWrite(9,HIGH);
    digitalWrite(8,HIGH);
    digitalWrite(10,LOW);
    digitalWrite(11,LOW);
  }
  else(digitalRead(sensorpir)== LOW);{
    digitalWrite(11,HIGH);
    digitalWrite(10,HIGH);
    digitalWrite(9,LOW);
    digitalWrite(8,LOW);
  }
}
