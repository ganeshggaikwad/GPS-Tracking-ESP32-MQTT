# GPS-Tracking-ESP32-MQTT
Asset (most commonly Vehicle) Tracking using GPS with MQTT connectivity.

# Hardware Used
1. ESP32 Development board
2. NEO-6MV2 GPS module
4. Breadboard
5. Jumper wires
6. Computer running Arduino IDE software.
7. USB micro cable to connect ESP32 development board to the computer.
8. A WiFi Hotspot

# Hardware Setupt and Connections
The GPS module will be powered with 3.3V power supply from ESP32.
It can communicates with the ESP32 via serial communication [we can use software serial channel] using the TX and RX pins available on the 4 pins header.
Connect the VCC pin of the GPS module to the ESP32 3.3V pin.
Connect the GPS ground pin to the ESP32 ground pin.
Now, connect the RX pin of the GPS module to the TX pin of the ESP32. Similarly, connect the TX pin of the GPS module to the RX pin of the ESP32 (RX and TX pins of the ESP32 are defined in the program/software).
Now, connect your ESP32 to the computer through a micro USB cable.
The ESP32 will be powered from the USB 5V.

# Libraries Used
1. TinyGPS++ Library - https://github.com/mikalhart/TinyGPSPlus
2. EspSoftwareSerial Library - https://github.com/plerup/espsoftwareserial/
3. PubSubClient library - https://github.com/asksensors/pubsubclient

# Conclusion
The GPS alone is a quiet difficult to understand device because it uses different security protocols and operation procedure. By connecting it to the cloud, it can be used for live tracking, smart Navigation system and Tracking applications. This repository described how to connect the GPS NEO-6MV2 module with the ESP32 via MQTT protocol to any of the cloud.

Please feel free to comment.
