# ArduinoCampana


int HombreBoton = 1;
int MujerBoton = 2;
int PlayBoton = 3;
int PausaBoton = 4;
int Round = 1;
void setup() {
  // put your setup code here, to run once:
pinMode(HombreBoton, INPUT);
pinMode(MujerBoton, INPUT);
pinMode(PausaBoton, INPUT);
pinMode(PlayBoton, INPUT);
}

void loop() {
  // put your main code here, to run repeatedly:
  buttonState1 = digitalRead(HombreBoton);
  buttonState2 = digitalRead(MujerBoton);
  buttonState3 = digitalRead(PlayBoton);
  buttonState4 = digitalRead(PausaBoton);

  // check if the pushbutton is pressed. If it is, the buttonState is HIGH:
  if (buttonState1 == HIGH) {
    // logica 1
    while(x<5){
   digitalWrite(9,HIGH);
   delay(200);
   digitalWrite(9,LOW);
   delay(200);
    x++;
 }
  } 
  if (buttonState2 == HIGH) {
    // logica 2
  }
  if (buttonState3 == HIGH) {
    // logica 3
  }
  if (buttonState4 == HIGH) {
    // logica 4
  }
}
