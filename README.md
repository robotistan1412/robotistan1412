int 
led=3, 
sensorpin=7; 
void setup() {
pinMode(led,OUTPUT); 
pinMode(sensorpin,INPUT); 
Serial.begin(9600); 

}

void loop() {
int data = digitalRead(sensorpin); 
Serial.println(data); 
if (data == 0) { 
  
  digitalWrite(led,HIGH); 
  }
  else{
    digitalWrite(led,LOW); 
    }

}
