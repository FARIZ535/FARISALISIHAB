# FARISALISIHAB
create, correct, improve, implement

const int potPin = 34;  // pin dari out potensio

void setup() {
  Serial.begin(115200);
}

void loop() {
  int potValue = analogRead(potPin);
  Serial.println(potValue);
  delay(100);
}
