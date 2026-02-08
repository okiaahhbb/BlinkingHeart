// 8 LED HEARTBEAT (side → center)
// Pins used: D2 to D9

int heart[] = {2,9,3,8,4,7,5,6};  // side theke center
int total = 8;

void setup() {
  for (int i = 0; i < total; i++) {
    pinMode(heart[i], OUTPUT);
  }
}

void loop() {
  // Build up (side → center)
  for (int i = 0; i < total; i++) {
    digitalWrite(heart[i], HIGH);
    delay(100);
  }

  // Double heartbeat
  for (int j = 0; j < 2; j++) {
    for (int i = 0; i < total; i++)
      digitalWrite(heart[i], LOW);
    delay(120);

    for (int i = 0; i < total; i++)
      digitalWrite(heart[i], HIGH);
    delay(120);
  }

  // Turn off slowly
  for (int i = 0; i < total; i++) {
    digitalWrite(heart[i], LOW);
    delay(80);
  }

  delay(600); // rest time
}
