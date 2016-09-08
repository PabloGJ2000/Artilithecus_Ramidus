/*
 * Visita www.moaisenergy.com
 * Creative Commons Reconocimiento-Compartir Igual 4.0 Internacional License
 * Última edición el 08/09/2016 por Pablo García Jaén
*/

int valor=0;
int dolor=0;
void setup() {
Serial.begin(9600);
pinMode(9,OUTPUT);
pinMode(10,OUTPUT);

pinMode(11, INPUT_PULLUP);
pinMode(2, INPUT);
}

void loop() {

dolor=digitalRead(11);

valor=digitalRead(2);
if((valor==0) && (dolor==1)) {
  digitalWrite(9,LOW);
  digitalWrite(10,LOW);
}
if((valor==1) && (dolor==1)) {
  digitalWrite(9,HIGH);
  digitalWrite(10,LOW);
}
if(dolor==0) {
  digitalWrite(9,LOW);
  digitalWrite(10,HIGH);
}
delay(10);
}
