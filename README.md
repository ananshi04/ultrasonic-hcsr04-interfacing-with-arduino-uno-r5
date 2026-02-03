# Ultrasonic Distance Sensor (HC-SR04) Example

## Description
Simple Arduino sketch that measures distance using an HC-SR04 ultrasonic sensor and prints the value to the serial monitor at 9600 baud.

## Hardware Required
\- Arduino board (Uno, Nano, etc.)  
\- HC-SR04 ultrasonic sensor  
\- Jumper wires  
\- Breadboard (optional)

## Wiring
Connect the sensor to the Arduino as follows:  
\- `VCC` \-> `5V`  
\- `GND` \-> `GND`  
\- `TRIG` \-> Arduino digital pin `9`  
\- `ECHO` \-> Arduino digital pin `10`

## Software / Build
\- Use the Arduino IDE, Arduino CLI, PlatformIO, or your preferred toolchain to compile and upload the sketch.  
\- The project source file is `src/main.cpp`. The sketch uses `Serial.begin(9600)` for output.

## Usage
1. Upload the sketch to the Arduino.  
2. Open the Serial Monitor at `9600` baud.  
3. The output will display lines like: `Distance: 12.34 cm`.

## Notes & Troubleshooting
\- Ensure `TRIG` and `ECHO` wiring matches the pin definitions in `src/main.cpp`.  
\- If readings are erratic, check sensor power and wiring connections.  
\- `pulseIn()` is blocking; for higher responsiveness consider non-blocking measurement patterns or averaging multiple readings.

## License
MIT License — see `LICENSE` (add if desired).
