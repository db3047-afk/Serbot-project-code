# Serbot-project-code
🤖 ESP32 Line Follower + Obstacle Avoider Robot

This project combines line-following and obstacle-avoidance functionalities into a single autonomous robot powered by the ESP32 microcontroller.
It uses IR sensors for line tracking and an ultrasonic sensor for obstacle detection, while the TB6612FNG motor driver controls the movement of two DC motors.

🚀 Features

Dual Functionality: Follows a black/white line and avoids obstacles automatically.

Autonomous Navigation: Makes real-time decisions based on sensor input.

Smart Obstacle Detection: Uses an ultrasonic sensor to detect and bypass objects.

Smooth Motor Control: Controlled using TB6612FNG motor driver with PWM signals.

Fully Compatible: Works on the ESP32 development board.

🧠 Working Principle

Line Following:

Two IR sensors detect the path (usually a black line on a white surface).

If both sensors detect black → move forward.

If left sensor on black → turn left.

If right sensor on black → turn right.

If both on white → stop.

Obstacle Avoidance:

Ultrasonic sensor continuously measures distance in front.

If an obstacle is detected within 15 cm, robot stops and checks alternate paths (left and right).

Chooses the side with more clearance and maneuvers around the obstacle.
