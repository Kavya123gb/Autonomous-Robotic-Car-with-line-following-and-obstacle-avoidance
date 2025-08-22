Autonomous Robotic Car with line following and obstacle avoidance  
📖 Overview
This project is a simple **robotic car** that follows a black line using IR sensors and avoids obstacles using an ultrasonic sensor.  
It combines line following and obstacle sensing into one compact Arduino-based system.  

🎯 Objective
- To design and build an Arduino-based robotic car that can move automatically.  
- To implement **line following** using IR sensors.  
- To add **obstacle detection and avoidance** using an ultrasonic sensor.  

✨ Key Features
- Dual IR sensors for line detection  
- Ultrasonic sensor (HC-SR04) for obstacle sensing  
- Automatic stop → reverse → turn on obstacle detection  
- Smooth motor control using PWM (L298N motor driver)  
- Works with Arduino UNO/Nano  

⚙️ Working
1. The IR sensors continuously check for the black line on a white surface.  
   - Both sensors on line → move forward  
   - Left sensor on line → turn left  
   - Right sensor on line → turn right  
2. The ultrasonic sensor checks distance ahead.  
   - If obstacle < set distance → car stops, moves back, turns, and continues.  
3. The motor driver (L298N) controls both motors for forward, backward, and turning movements.


