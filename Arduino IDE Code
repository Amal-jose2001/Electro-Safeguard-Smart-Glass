#define Buz 6
#define Relay A5
#define EYE A3
String MSG;
int Time = 0;
Void setup() {
Serial.begin(9600);
pinMode(EYE, INPUT);
pinMode(Buz, OUTPUT);
pinMode(Relay, OUTPUT);
digitalWrite(Relay, LOW);
}
Void loop() {
If (digitalRead(EYE) == 0 ) {
Time++;
Delay(1000);
If (Time > 2) {
digitalWrite(Relay, HIGH);
Time = 0; 
Serial.println(“AT”);
Delay(200);
Serial.println(“AT+CMGF=1”);
Delay(200);
Serial.println(“AT+CMGS=\"+917306424906\”\r”);
Delay(200);
MSG = “THE DRIVER IS FATIGUE!”;
Serial.println(MSG);
Delay(200);
Serial.println((char)26);
Delay(200);
digitalWrite(Buz, HIGH);
while (1);
}
} 
Else{
Time=0;
}
