# HOME-AUTOMATION-WITH-BLUETOOTH

**COMPANY**: CODTECH IT SOLUTIONS

**NAME**: RIFANA NAZREEN A

**INTERN ID**:CT04DH23

**DOMAIN**: EMBEDDED SYSTEMS

**DURATION**: 4 WEEKS

**MENTOR**: NEELA SANTHOSH

DESCRIPTION:

This project is a Bluetooth-controlled home automation system using an Arduino Uno. It enables the control of a light, bulb, and fan by sending serial commands through a Bluetooth module (not shown in the image but typically connected to RX and TX pins).

In the circuit, three LEDs represent appliances:

* The light is connected to digital pin 2
* The bulb is connected to digital pin 3
* The fan is connected to digital pin 5

Each LED is connected in series with a resistor to limit current, and their grounds are connected to the Arduino GND.

The Arduino code defines three pins as outputs and reads characters received over the serial interface. When a specific character is received, the corresponding appliance turns on or off:

* 'A' turns on the light; 'a' turns it off
* 'B' turns on the bulb; 'b' turns it off
* 'C' turns on the fan; 'c' turns it off

Serial.begin(9600) starts serial communication at 9600 baud. The Serial.read() function listens for incoming characters. A switch-case structure processes each command, and feedback is sent back to the serial monitor using Serial.println().

This system can be operated through a serial monitor or a Bluetooth terminal app on a phone, making it suitable for wireless control of simple appliances in a smart home prototype.

OUTPUT:

<img width="1201" height="663" alt="Image" src="https://github.com/user-attachments/assets/2d9e5ca3-bafc-46db-bd78-c0b859727e69" />
