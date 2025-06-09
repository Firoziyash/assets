# Arduino Basics for Beginners

![Arduino Logo](https://www.arduino.cc/en/pub/skins/arduinoWide/img/ArduinoLogo-1.svg)

## What is Arduino?
Arduino is an open-source electronics platform based on easy-to-use hardware and software. It's perfect for beginners to learn electronics and programming.

## Basic Components
1. **Arduino Board** (Uno, Nano, Mega, etc.)
2. **USB Cable** (for power and programming)
3. **Breadboard** (for prototyping circuits)
4. **Jumper Wires**
5. **LEDs, Resistors, Sensors** (basic components to start with)

## Setting Up Arduino IDE
1. Download Arduino IDE from [arduino.cc](https://www.arduino.cc/en/software)
2. Install the software
3. Connect your Arduino via USB
4. Select the correct board and port in Tools menu

## Your First Program: Blink LED

```arduino
// The setup function runs once when you press reset or power the board
void setup() {
  // Initialize digital pin LED_BUILTIN as an output
  pinMode(LED_BUILTIN, OUTPUT);
}

// The loop function runs over and over again forever
void loop() {
  digitalWrite(LED_BUILTIN, HIGH);  // Turn the LED on
  delay(1000);                       // Wait for a second
  digitalWrite(LED_BUILTIN, LOW);   // Turn the LED off
  delay(1000);                       // Wait for a second
}
