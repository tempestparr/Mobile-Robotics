# Mobile-Robotics
### All challenges use the Lego education EV3 kit and RobotC programming language.

## Challenge 1

### Objectives: 
- Construct a robot using the Lego education EV3 kit
- Program your robot to display multiple layered behaviors
- Work in a team to creatively design and implement a project

### Design, construct, program, test, and demonstrate a mobile robot with the following behaviors:
- Wandering : implement a biased random walk (or drunken sailor walk) where the bot will zig-zag in a semi-random pattern with a generally forward motion.
- Object Detection and Reaction : use bumpers to detect obstacles in front of the robot. If the right side bumper is depressed, the bot backs up, turns left, and then resumes wandering. Similarly, if the left side bumper is depressed, the bot will perform a mirrored response. If both bumpers are depressed within 10ms of one another, the bot makes a sound, backs up, pauses, and turns in a random direction and resumes wandering.

## Challenge 2

### Objectives:
- Learn to use light sensors and ultrasonic (sonar) sensors
- Learn to dynamically arbitrate among several layered behaviors

### Design, construct, program, test, and demonstrate a mobile robot with the following behaviors:
- Wandering : as implemented in Challenge 1
- Line Following : use light sensors to detect a black line on the floor and follow the line to the end, make a sound, and then resume wandering
- Object Dectection and Approach : using ultrasonic sensors, detect an object within 3 feet, approach the object within 1 inch at a speed proportional to the distance to the object, stop, back up, turn a random direction away from the object, and then resume wandering.

## Challenge 3

### Objectives:
- Use at least 5 sensors
- Use 2 EV3 bricks which will communicate via Bluetooth or Wi-Fi

### Design, construct, program, test, and demonstrate a mobile robot with the following behaviors:
- Wandering : as implemented in Challenge 1
- Object Detection and Reaction : as implemented in Challenge 1
- Object Detection and Approach : as implemented in Challenge 2
- Patch feeding : once on a patch, the bot should not leave unless it detects an object, is frightened by
a flash of light, or has fed until it is “full”. Once full, the bot must return to wandering. While the bot is feeding, its energy level increases. It takes 2 minutes of feeding to become full. When not on a patch feeding, the energy level decrements. Low energy levels are interpreted as "hunger". When the energy level is below a certain point, it is in a hungry state. Feeding involves continuously moving in a non-repetitive way (wandering) on the patch.
- Escape : detect flashes of light and run away from the light source. The robot will gradually habituate to the light flashes, decreasing the speed at which it runs away, and eventually will fully habituate if exposed to light flashes often enough. After time with no light flash exposure, the bot will restore its initial response behavior.
- Death : the bot will play a sound and cease all activity if the energy level ever reaches zero
