int buzzerPin = 9;
unsigned long startTime;
boolean sixMinutesPassed = false;

void setup() {
  pinMode(buzzerPin, OUTPUT);
  startTime = millis(); // Record the start time
}

void loop() {
  unsigned long currentTime = millis();
  
  if (!sixMinutesPassed) {
    // Run the 6-minute program
    if (currentTime - startTime <= 360000) { // Check if 6 minutes have not passed
      digitalWrite(buzzerPin, HIGH);
      delay(3);
      digitalWrite(buzzerPin, LOW);
      delay(20);
      digitalWrite(buzzerPin, HIGH);
      delay(3);
      digitalWrite(buzzerPin, LOW);
      delay(22);
      digitalWrite(buzzerPin, HIGH);
      delay(3);
      digitalWrite(buzzerPin, LOW);
      delay(24);
      digitalWrite(buzzerPin, HIGH);
      delay(3);
      digitalWrite(buzzerPin, LOW);
      delay(26);
      digitalWrite(buzzerPin, HIGH);
      delay(3);
      digitalWrite(buzzerPin, LOW);
      delay(28);
      digitalWrite(buzzerPin, HIGH);
      delay(3);
      digitalWrite(buzzerPin, LOW);
      delay(30);
      digitalWrite(buzzerPin, HIGH);
      delay(3);
      digitalWrite(buzzerPin, LOW);
      delay(32);
    } else {
      sixMinutesPassed = true; // Set the flag to indicate 6 minutes have passed
      startTime = currentTime; // Reset the start time for the next program
    }
  } else {
    // Run the 30-minute program
    if (currentTime - startTime <= 1800000) { // Check if 30 minutes have not passed
      digitalWrite(buzzerPin, HIGH);
      delay(3);
      digitalWrite(buzzerPin, LOW);
      delay(20);
      digitalWrite(buzzerPin, HIGH);
      delay(3);
      digitalWrite(buzzerPin, LOW);
      delay(18);
      digitalWrite(buzzerPin, HIGH);
      delay(3);
      digitalWrite(buzzerPin, LOW);
      delay(16);
      digitalWrite(buzzerPin, HIGH);
      delay(3);
      digitalWrite(buzzerPin, LOW);
      delay(14);
      digitalWrite(buzzerPin, HIGH);
      delay(3);
      digitalWrite(buzzerPin, LOW);
      delay(12);
      digitalWrite(buzzerPin, HIGH);
      delay(3);
      digitalWrite(buzzerPin, LOW);
      delay(8);
      digitalWrite(buzzerPin, HIGH);
      delay(3);
      digitalWrite(buzzerPin, LOW);
      delay(6);
    } else {
      // End the program after both durations have passed
      digitalWrite(buzzerPin, LOW); // Turn off the buzzer
      while (true) {} // Endless loop to halt the program
    }
  }
}
