🚦 STM32 LED + Potentiometer Project

This project demonstrates how to use the ADC (Analog-to-Digital Converter) of the STM32 Nucleo-F103RB board to control the speed of an LED chaser using a potentiometer.

The potentiometer generates an analog voltage (0-3.3V), which the STM32 reads and converts to a digital value (0–4095). That value is then mapped to a delay, making the LED chase speed adjustable in real time.

🧰 Hardware Used
Component	Quantity
STM32 Nucleo-F103RB	1
Breadboard	1
LEDs	4
120Ω Resistors	4
Potentiometer (10kΩ recommended)	1
Jumper Wires	As needed
🔌 Wiring Diagram
LED Connections
LED	STM32 Pin	Series Resistor	Ground
LED1	PA5	220Ω	GND
LED2	PA6	220Ω	GND
LED3	PA7	220Ω	GND
LED4	PA8	220Ω	GND
Potentiometer Wiring
Potentiometer Pin	Connect To
Left side	GND
Right side	3.3V
Middle (Wiper)	PA0 (ADC Input)
⚙️ CubeMX Configuration
Setting	Value
Pin PA5-PA8	GPIO Output
Pin PA0	ADC Input Mode
ADC Resolution	12-bit
Clock	Default settings are fine
📌 Features

Adjustable LED chase speed using the potentiometer

Non-blocking delay based on ADC reading

Beginner-friendly embedded example

🧪 How It Works

Read analog voltage from potentiometer using ADC.

Convert ADC value (0-4095) into a usable delay.

Cycle LEDs in sequence using the delay.

Repeat forever in the main loop.

▶️ How to Run

Flash the program to STM32 using STM32CubeIDE.

Rotate the potentiometer.

Watch the LED chase speed change!

🛠️ Future Improvements

📍 PWM-based LED brightness control

📍 OLED/Serial message showing ADC value

📍 CAN data output for real vehicle logging

📚 Learning Outcome

This project teaches:

GPIO control

ADC configuration and reading

Mapping sensor values

Embedded programming workflow

🧑‍💻 Author

Adarsh Behera
Aspiring AUTOSAR & Embedded Engineer 🚀
