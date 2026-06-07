This project is a real-time, battery-powered mobile robot controlled wirelessly via Bluetooth. 

It utilizes the hardware interrupt capabilities of the STM32 to handle user commands without blocking the main processor.

Interrupt-Driven Communication: Uses STM32's hardware interrupts (HAL_UART_Receive_IT) for non-blocking, real-time Bluetooth command processing.


//KEY FEATURES//
Smart Power Management: Steps up a single 3.7V Li-ion battery to a stable 12.2V using a Boost Converter to fully power the motors.

Dual H-Bridge Control: Drives DC motors using the L298N driver based on incoming direction commands.

Visual Feedback: Toggles an onboard LED on every successful data reception to show active link connection.


//HARDWARE COMPONENTS//
Microcontroller: STM32F407G-DISC1 (ARM Cortex-M4)

Power Management: 3.7V Li-ion Battery & DC-DC Boost Converter (Regulated to 12.2V)

Motor Driver: L298N Dual H-Bridge Driver

Connectivity: HC-05/HC-06 Bluetooth Module (UART @ 9600 Baud Rate)

Firmware Framework: STM32CubeIDE / HAL (Hardware Abstraction Layer)


//COMMAND SET//
F / f / 1 : Move Forward

R / r / 2 : Move Backward-Reverse

S / s / 0 : Stop
