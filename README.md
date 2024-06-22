# SLASH-MARK-TASK-Step 1: Gather all the components on the Digital Board or Physical Table.

Micro Servo:

Step 2: Connect the Ground terminal of each to the GND pin of the Arduino.

Step 3: Connect the Power terminal of each to the 5V pin of the Arduino.

Step 4: Connect the Signal terminal of it to the 4, 5, 6, & 7 number pins of the Arduino, respectively.

Source Code
#include <Servo.h>
Servo s1, s2, s3, s4;
void setup()
{
s1.attach(4);
s1.write(90);
s2.attach(5);
s2.write(90);
s3.attach(6);
s3.write(90);
s4.attach(7);
s4.write(90);
}
void loop()
{
s1.write(90);
s2.write(90);
s3.write(90);
s4.write(90);
delay(10000);


s1.write(0);
s2.write(0);
s3.write(0);
s4.write(0);
delay(10000);
}
Explanation of the Code
1. First, we need to include the Servo library.

2. After that, we declared the objects of each servo.

3. In the setup function, we have attached each servo to the pin number to which they are connected and written each to 90 degrees initially.

4. In the loop function, we are changing the opposite servo degrees to 0 to 90 and 90 to 0, respectively, after a time period of 10 seconds, as used in the delay function.

Output
We have demonstrated the final output of this smart traffic management system project below.

Smart Traffic Management System with Arduino

On starting the simulation, the servo motor will give way to each path for some stipulated time.

2
