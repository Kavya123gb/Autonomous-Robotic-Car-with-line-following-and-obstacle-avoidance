This project is a Raspberry Pi Pico–based robotic car that can follow a black line using IR sensors and avoid obstacles using an ultrasonic sensor.
It combines line following + obstacle avoidance in one compact embedded system.

🎯 Objective

To design and build an autonomous robotic car using Raspberry Pi Pico.

To implement line following using IR sensors.

To implement obstacle detection and avoidance using an ultrasonic sensor.

✨ Key Features

Dual IR sensors for line detection

Ultrasonic sensor (HC-SR04) for obstacle sensing

Automatic stop → reverse → turn → resume on obstacle detection

Smooth motor control using PWM (L298N motor driver)

Compact, low-cost, and easy to build using Raspberry Pi Pico

⚙️ Working

The IR sensors continuously check for the black line on a white surface.

Both sensors on line → move forward

Left sensor on line → turn left

Right sensor on line → turn right

The ultrasonic sensor checks the distance ahead.

If distance < threshold → car stops, moves back, turns, and continues.

The L298N motor driver controls both motors for forward, backward, and turning movements with PWM signals.

📌 Pin Configuration (Raspberry Pi Pico)
Component	Pico Pin (GPIO)
Left IR Sensor	GP26 (ADC0)
Right IR Sensor	GP27 (ADC1)
Ultrasonic TRIG	GP3
Ultrasonic ECHO	GP2
L298N ENA (Left PWM)	GP16
L298N IN1 (Left)	GP17
L298N IN2 (Left)	GP18
L298N ENB (Right PWM)	GP19
L298N IN3 (Right)	GP20
L298N IN4 (Right)	GP21
🔧 Components Used

Raspberry Pi Pico

L298N Motor Driver

2 × IR Sensors

1 × Ultrasonic Sensor (HC-SR04)

2 × DC Motors + Wheels

Robot Chassis + Caster wheel

Battery Pack (7.4V–12V)
🚀 How to Run

Install Thonny IDE on your computer.

Connect Raspberry Pi Pico via USB.

Copy the above code into Thonny and save as main.py on the Pico.

Assemble the car as per pin configuration.

Place it on a track with a black line on white surface.

Power the Pico with a battery pack → Car starts moving autonomously.

Conclusion
This project successfully demonstrates the design and implementation of an autonomous robotic car using Raspberry Pi Pico.
The car is capable of:

Following a line accurately using IR sensors.

Detecting and avoiding obstacles using an ultrasonic sensor.

Controlling motors smoothly with PWM through the L298N driver.

By combining line following and obstacle avoidance, the system achieves basic autonomous navigation on a predefined track.

This project not only highlights the potential of Raspberry Pi Pico in robotics, but also provides a low-cost and scalable platform for future improvements such as:

Bluetooth/WiFi remote control

Speed optimization

Multi-sensor fusion for better accuracy

In conclusion, the robotic car is a compact, reliable, and practical prototype that can be further enhanced for real-world autonomous vehicle applications. 🚗✨
