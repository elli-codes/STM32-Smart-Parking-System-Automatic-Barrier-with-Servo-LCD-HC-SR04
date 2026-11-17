# STM32-Smart-Parking-System-Automatic-Barrier-with-Servo-LCD-HC-SR04 🚗


A mini smart parking system based on the STM32F103C8T6 (Blue Pill) microcontroller. This project uses an HC-SR04 ultrasonic sensor to detect approaching vehicles, a servo motor to control the parking barrier, and a 16x2 LCD to display the remaining parking capacity.

The parking lot has a limited capacity of 2 vehicles. When a vehicle approaches, the system checks whether a parking space is available. If the parking lot is not full, the barrier opens to allow the vehicle to enter, and the available capacity decreases by one.

When all parking spaces are occupied, the barrier remains closed and the LCD displays a parking-full message.

🎥 Project Demo

Watch the video demonstration to see how the system detects vehicles, controls the barrier, and updates the available parking capacity.

✨ Features

Vehicle Detection: Detects approaching vehicles using the HC-SR04 ultrasonic sensor.

Automatic Barrier Control: Uses a servo motor to open and close the parking gate.

Capacity Management: Starts with 2 available parking spaces and decreases the capacity after each vehicle enters.

LCD Display: Shows the parking status and remaining capacity on a 16x2 LCD.

Full Parking Detection: Prevents vehicle entry when the parking lot reaches its maximum capacity.

Real-Time Response: Updates the parking status based on ultrasonic sensor measurements.

⚙️ How It Works

The system follows these steps:

The HC-SR04 sensor continuously measures the distance in front of the parking entrance.

When an approaching vehicle is detected (distance below 20 cm), the microcontroller checks the available capacity.

If at least one parking space is available:

The servo motor opens the barrier.

The vehicle is allowed to enter.

The available capacity decreases by one.

The LCD displays the updated capacity.

After a short delay, the barrier closes.

If the capacity reaches zero:

The servo motor keeps the barrier closed.

The LCD displays Parking is full.

No additional vehicle is allowed to enter.

📌 Project Scope

This version focuses on vehicle entry detection and parking capacity management. The available capacity decreases when a vehicle enters. Automatic vehicle exit detection and capacity restoration are not implemented in this version.



💻 Software and Development Tools

STM32CubeMX

IAR Embedded Workbench

STM32 HAL Library

Embedded C

🖥️📽️YouTube video link:https://youtu.be/MxsXAVWJNxc?si=Lj1Xz46T_Le-cZLg

