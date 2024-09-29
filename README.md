# FARISALISIHAB
create, correct, improve, implement
const int potPin = 32;  // pin input dari pot

void setup() {
  Serial.begin(115200);
}

void loop() {
  int sensorValue = analogRead(potPin);
  int percentage = map(sensorValue, 0, 4095, 0, 100);
  Serial.print("Potentiometer value: ");
  Serial.print(percentage);
  Serial.println("%");
  delay(500);
}
