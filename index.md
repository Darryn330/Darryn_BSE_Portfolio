# BlueStamp Self Driving Car
Recently, self-driving cars have moved from something coming from a futuristic timeline to real world testing. Vehicles such as Waymo have now become increasingly common in society, taking over the role of drivers. The project below showcases a simple way to build a self-driving car that allows the user to control it with a device, or have it avoid obstacles in its way. 

```HTML 
<!--- This is an HTML comment in Markdown -->
<!--- Anything between these symbols will not render on the published site -->
```

| **Engineer** | **School** | **Area of Interest** | **Grade** |
|:--:|:--:|:--:|:--:|
| Darryn K | Lowell High School | Game Designer | Incoming Freshman

<!--**Replace the BlueStamp logo below with an image of yourself and your completed project. Follow the guide [here](https://tomcam.github.io/least-github-pages/adding-images-github-pages-site.html) if you need help.**-->

![Headstone Image](logo.svg)
  
# Final Milestone

<!--**Don't forget to replace the text below with the embedding for your milestone video. Go to Youtube, click Share -> Embed, and copy and paste the code to replace what's below.**

<iframe width="560" height="315" src="https://www.youtube.com/embed/F7M7imOVGug" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>

For your final milestone, explain the outcome of your project. Key details to include are:
- What you've accomplished since your previous milestone
- What your biggest challenges and triumphs were at BSE
- A summary of key topics you learned about
- What you hope to learn in the future after everything you've learned at BSE-->



# Second Milestone
<iframe width="560" height="315" src="https://www.youtube.com/embed/yrKTVxtxmPo?si=Vk0Km7bvmR98Q2ed" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

### Description: 
Now that the IR obstacle avoidance sensors and the ultrasonic sensor were finally attatched and coded, I was able to get it to back away from objects whenever it sensed it. In the previous milestone, I hadn't yet added these sensors, so it would bump into everything when I tried to make it move. Now, I'm able to make it follow my hand, and back away from any obstacles in its way. Another sensor type object I added was the line tracking sensor which could make the car follow a line. Additionally, I was able to make the self-driving car use certain sensors and codes whenever the corresponding button was pressed. For example, if I pressed the EQ button on the remote controller, it would automatically switch to folowing my hand instead of following the remote controller which it uses by default. With the measurements from both sensors, I was able to have the self driving car follow my hand. As long as it was within 5 inches from the sensor, it would receive the signal, and either move forward or stop. For example, if my hand were too close to the sensor, it wouldn't move, but if my hand stayed approximately 5 inches away from the sensor, it would continue following me. Another feature I added was the remote control. To begin using it, I first added the IR receiver to the breadboard and attatched it to pin 12 and VCC and GND so it would receive the remote controllers infrared signals. When a certain button was pressed, it would either stop, move, speed up, or slow down. (Refer to Schematic 2 for wiring schematic) 

### Challenges: 
It was challenging to put together code because I had several lines of code used for different functions on my car, and I had to take pieces out of each code and add it to button functions on the remote controller. Due to the movement codes clashing with one another, the car became confused from all the different directions it was receiving, so it didn't work. Eventually, I was able to fix it by deleting the commands that made the car constantly move forward at all times, or move backwards when it senses an object. Then, I deleted end brackets ('}') which were causing the code to be confused as I was asking it to end twice. (Refer to Milestone 2 code)

### Plan for the project: 
My plan for the next milestone would be to make it gesture controlled, as I've always seen people using gesture controlled cars as a kid. I thought it was fascinating how they were able to control the movement of an object like it was an extension of themselves. 

# First Milestone
<iframe width="560" height="315" src="https://www.youtube.com/embed/YdEHZaryFaI?si=4RKEKhnF_nQri2_l" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

### Description: 
For my first milestone, I started with the acrylic board first, adding motors, then wheels to it so I have a shell to test my code on. Next, I started wiring the car to the Arduino Uno board which would allow code to reach different components. Without an Arduino Uno board, there would be nothing I could transmit code through, therefore giving me an empty shell. Due to the lack of slots to fit each wire in on my Arduino Uno board, I needed to add a mini breadboard, so I could have each wire function properly. The breadboard gave me room to connect the power and ground pins into specific rows which contained space to put more wires. So far, I've made it move backward, forwards, and rotate in a constant loop. (Refer to schematic 1)

### Challenges: 
A challenge I had was putting the wires together, as I've never really worked with wires before, so I kept on running out of place to put them, and almost made one of my IR obstacle avoidance sensors short circuit due to the wires being swapped. Afterwards, I learned that I had to look at the labels next to the pins to know where to place them. During my first week here, I learned that I could set certain rows for 5V and GND pins by connecting them to the breadboard. As the two rows began filling up with wires, I connected those rows to a different spot on the breadboard, so I have enough space for all my wires. (Refer to Schematic 1)

### Plan for the project: 
My plan for this project would be to finish coding the sensors, and begin making it remote controlled, or have it travel to a desired destination. 

# Starter Project
<iframe width="560" height="315" src="https://www.youtube.com/embed/4H36yDGcPsc?si=E1qQTdqLzmyNdy_T" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

### Description: 
My starter project was the RGB slider. The RGB slider contains 3 lightbulbs within another. Whenever the user flicked a certain slider, the colored bulb the slider corresponded to increased its intesity. Additionally, it required me to solder on 29 joints to mend the pieces together. Soldering used a paintbrush like tool, which you had to hold like a pencil, and carefully melt soldering iron on the desired area. 

### Challenges: 
A challenge I faced was when I accidentally soldered 2 parts together. Due to how close the 2 areas were, the liquidated solder combined, and formed a singular ball. Luckily, there was a device that could suck all the liquid up, so I remelted the soldering iron, and used the device. Another problem that occured was that the wires were too long, and the scizzors wouldn't fit. Eventually, after a while, I was finally able to cut uneccessary pieces off. 

### Next Steps: 
My next steps are to build the self-driving car, and code it. The project I'm currently doing is the self-driving car, which requires me to build the shell, and code it to avoid obstacles. Building the shell would allow me to have something to test my code in, meaning that I can identify problems in my code, and in the shell. Additionally, I need to add modifications to my car. A few modifications I'm thinking about are to make it gesture controlled, have it jump, or give it a nitro booster. 

# How it works: 

### Overview
I added different sensors such as the ultrasonic sensor and the IR obstacle avoidance sensors. The ultrasonic sensor transmits an ultrasonic wave through one side which hits an object, eventually receiving the wave through the other side. It uses the amount of time it takes to receive the wave after transmitting it to measure the distance between itself and another object. On the other hand, instead of using an ultrasonic wave, the IR obstacle avoidance sensors use infrared light to measure its distance from an object. It sends an infrared ray which reflects off of an object and comes back to the receiver. If there is no object in front of it, the infrared ray wouldn't reflect off anything and would continue traveling. Additionally, the screw on the top of the sensors can be used to adjust its sensitivity. (Refer to schematic 1 for a better idea of how it looks) 

#### Ultrasonic Sensor
As said previously, the IR obstacle avoidance sensors and ultrasonic sensor send a wave or ray in front of it, which bounces off an object is received by the sensor. The ultrasonic sensor has 4 pins named VCC(power), GND(ground), TRIG(trigger), and ECHO. Using wires, I connected TRIG and ECHO to pins 3 and 4 on the Arduino Uno R3 board. I called upon the trigger and echo pins on the ultrasonic module using code so I could receive data from the ultrasonic wave it sends. With the code 'Serial.print' I printed how far the ultrasonic sensor was from another object on a tool called the Serial Monitor which is built into the Arduino IDE coding platform. The echo pin was set as an input, meaning it receives the wave, while the trigger pin was set as an output, so it's the side that transmits the wave. 

#### IR Obstacle Avoidance 
As for the IR obstacle avoidance module sensors, I used code to set the pin values of the leftIR and rightIR to 7 and 8. Each sensor has 3 pins saying VCC(power), GND(ground), and OUT(output). The OUT pin is a digital output signal indicating whether an obstacle is detected or not. Therefore, I had to wire both sensor's OUT pins to their corresponding pins so the code could go to the correct modules. When the 2 sensors detected an object close to it, it made the wheel opposite of it spin backward making it turn away from the object. When both sensors were obstructed, the car moved backwards. 

The line tracking sensor used infrared light to detect the contrast between the line and the area around it. It shoots out infrared light in front of it and uses the reflected light from the ground to see where the line is. Usually, a darker area would reflect less light, and a lighter background reflects more. Because lines are usually black, they would reflect less light, so the car would know exactly what to follow. 

Finally, the last tool I used for my self driving car was a remote control. The remote control uses an IR receiver to receive infrared transmissions from the remote controller. With 21 buttons on it, I was able to set different functions for each button. For example, the fast forward and rewind buttons activated the ultrasonic or IR obstacle avoidance sensors while the numbered buttons allowed me to control the direction it goes. 

# Schematics

## Module 1 Schematic
Schematic 2: 
![Second schematics Image](https://raw.githubusercontent.com/Darryn330/Darryn_BSE_Portfolio/refs/heads/gh-pages/Module%202.png)

Schematic 1:
![Schematics Image](https://raw.githubusercontent.com/Darryn330/Darryn_BSE_Portfolio/refs/heads/gh-pages/Module%201%20screenshot.png)

# Code

### Milestone 2 Code
```c++
#include <IRremote.h>

const int IR_RECEIVE_PIN = 12;                                      // Define the pin number for the IR Sensor

const int A_1B = 5;                                                 //sets motors to certain pins
const int A_1A = 6;

const int B_1B = 9;
const int B_1A = 10;

const int trigPin = 3;                                              //the wire connecting to pin 3 
const int echoPin = 4;                                              //wire connecting to pin 4

const int rightIR = 7;                                              //code is transmitted to pin 7
const int leftIR = 8;                                               //code is transmitted to pin 8

int speed = 150;                                                    //declares the speed variable

void setup() {
  Serial.begin(9600);                                               //starts serial monitor

  //motor
  pinMode(A_1B, OUTPUT);                                            //sets the motors to outputs
  pinMode(A_1A, OUTPUT);
  pinMode(B_1B, OUTPUT);
  pinMode(B_1A, OUTPUT);

  //IR remote
  IrReceiver.begin(IR_RECEIVE_PIN, ENABLE_LED_FEEDBACK);            // Start the IR receiver // Start the receiver
  Serial.println("REMOTE CONTROL START");                           //prints the string in the serial monitor

    //ultrasonic
  pinMode(echoPin, INPUT);                                          //set echo pin as an input
  pinMode(trigPin, OUTPUT);                                         //set trigger pin as an output

    //IR obstacle
  pinMode(leftIR, INPUT);                                           //sets the IR obstacle avoidance modules to inputs
  pinMode(rightIR, INPUT);

}

void loop() {

  if (IrReceiver.decode()) {                                        //checks if IR signal has been received and decoded
    //    Serial.println(results.value,HEX);
    String key = decodeKeyValue(IrReceiver.decodedIRData.command);  //decodes the IR command and stores it in the key variable
    if (key != "ERROR") {                                           //checks if the signal is not an error
      Serial.println(key);

      if (key == "+") {                                             //When a key is pressed on your remote control, the IR receiver will know what key is pressed, making the car move according to the corresponding key. 
        speed += 50;
        Serial.print("Speed up");
        Serial.println ("");
      } else if (key == "-") {
        speed -= 50;
        Serial.print("Speed down");
        Serial.println ("");
      } else if (key == "2") {
        moveForward(speed);
        delay(1000);
        Serial.print("Move forward");
        Serial.println ("");
      } else if (key == "1") {
        moveLeft(speed);
        Serial.print("Move left");
        Serial.println ("");
      } else if (key == "3") {
        moveRight(speed);
        Serial.print("Move right");
        Serial.println ("");
      } else if (key == "4") {
        turnLeft(speed);
        Serial.print("Turn left");
        Serial.println ("");
      } else if (key == "6") {
        turnRight(speed);
        Serial.print("Turn right");
        Serial.println ("");
      } else if (key == "7") {
        backLeft(speed);
        Serial.print("Moving backleft");
        Serial.println ("");
      } else if (key == "9") {
        backRight(speed);
        Serial.print("Moving backright");
        Serial.println ("");
      } else if (key == "8") {
        moveBackward(speed);
        delay(1000);
        Serial.print("Moving back");
        Serial.println ("");
      } else if (key == "POWER") {
        stopMove();
        Serial.print("Stopped");
        Serial.println("");
        delay (2000);

      }

      if (speed >= 255) {                                      //sets max speed to 255
        speed = 255;
      }
      if (speed <= 0) {                                        //sets minimum speed to 0
        speed = 0;
      }
      delay(500);
      stopMove();
    }

    IrReceiver.resume();                                      // Enable receiving of the next value
  }

  int left = digitalRead(leftIR);                             // 0: Obstructed   1: Empty
  int right = digitalRead(rightIR);                           //the numbers above mean that if 0 is printed, there is an obstacle, otherwise, 1 is printed
  
  int speed = 150;

  if (!left && right) {                                      //if left is low, and if the right is empty, it would move to the right
    backLeft(speed);
  } else if (left && !right) {                              //if left is empty and right isn't, move to left
    backRight(speed);
  } else if (!left && !right) {                             //if both are empty, move backward
    moveBackward(speed);
    delay(1000);
  }

  float distance = readSensorData();                        //reads the distance and returns it, stores it in a variable called distance
  Serial.print (distance);
  delay(2000);
                                                            // if (distance > 25) { //if the distance is greater than 25 cm then move forward with a speed of 200
                                                            //   moveForward(200);
                                                            // }
  if (distance < 10 && distance > 2) {                      //otherwise, if the distance is less than 10 and greater than 2: move backwards at a speed of 200
    moveBackward(200);
  } else {
    stopMove();
  }
}

float readSensorData() {
  digitalWrite(trigPin, LOW);                               //turning sensor off for 2 microseconds
  delayMicroseconds(2);
  digitalWrite(trigPin, HIGH);                              //turning sensor on for 10 microseconds
  delayMicroseconds(10);
  // digitalWrite(trigPin, LOW);                            //turns sensor off 
  float distance = pulseIn(echoPin, HIGH) / 58.00;          //Equivalent to (340m/s*1us)/2
  return distance;                                          //reads echoPin and divides it by 58 after returning it
}

void moveForward(int speed) {
  analogWrite(A_1B, 0);
  analogWrite(A_1A, speed);
  analogWrite(B_1B, speed);
  analogWrite(B_1A, 0);
}

void moveBackward(int speed) {
  analogWrite(A_1B, speed);
  analogWrite(A_1A, 0);
  analogWrite(B_1B, 0);
  analogWrite(B_1A, speed);
}

void turnRight(int speed) {
  analogWrite(A_1B, speed);
  analogWrite(A_1A, 0);
  analogWrite(B_1B, speed);
  analogWrite(B_1A, 0);
}

void turnLeft(int speed) {
  analogWrite(A_1B, 0);
  analogWrite(A_1A, speed);
  analogWrite(B_1B, 0);
  analogWrite(B_1A, speed);
}

void moveLeft(int speed) {
  analogWrite(A_1B, 0);
  analogWrite(A_1A, speed);
  analogWrite(B_1B, 0);
  analogWrite(B_1A, 0);
}

void moveRight(int speed) {
  analogWrite(A_1B, 0);
  analogWrite(A_1A, 0);
  analogWrite(B_1B, speed);
  analogWrite(B_1A, 0);
}

void backLeft(int speed) {
  analogWrite(A_1B, speed);
  analogWrite(A_1A, 0);
  analogWrite(B_1B, 0);
  analogWrite(B_1A, 0);
}

void backRight(int speed) {
  analogWrite(A_1B, 0);
  analogWrite(A_1A, 0);
  analogWrite(B_1B, 0);
  analogWrite(B_1A, speed);
}

void stopMove() {
  analogWrite(A_1B, 0);
  analogWrite(A_1A, 0);
  analogWrite(B_1B, 0);
  analogWrite(B_1A, 0);
}


String decodeKeyValue(long result)                         //if a certain button is pressed, it returns what button is pressed, and uses the code for the button
{
  switch(result){
    case 0x16:
      return "0";
    case 0xC:
      return "1"; 
    case 0x18:
      return "2"; 
    case 0x5E: 
      return "3";
    case 0x8:
      return "4"; 
    case 0x1C:
      return "5"; 
    case 0x5A:
      return "6"; 
    case 0x42:
      return "7"; 
    case 0x52:
      return "8"; 
    case 0x4A:
      return "9"; 
    case 0x9:
      return "+"; 
    case 0x15:
      return "-"; 
    case 0x7:
      return "EQ"; 
    case 0xD:
      return "U/SD";
    case 0x19:
      return "CYCLE";         
    case 0x44:
      return "PLAY/PAUSE";   
    case 0x43:
      return "FORWARD";   
    case 0x40:
      return "BACKWARD";   
    case 0x45:
      return "POWER";   
    case 0x47:
      return "MUTE";   
    case 0x46:
      return "MODE";       
    case 0x0:
      return "ERROR";   
    default :
      return "ERROR";
    }
}

```
### Milestone 1 Code
```c++
const int A_1B = 5;                   //set motors to certain pins
const int A_1A = 6;
const int B_1B = 9;
const int B_1A = 10;

void setup() {
  pinMode(A_1B, OUTPUT);             //set motors as outputs
  pinMode(A_1A, OUTPUT);
  pinMode(B_1B, OUTPUT);
  pinMode(B_1A, OUTPUT);
}

void loop() {                       //makes it move in this pattern forever
  moveForward();
  delay(2000);
  stopMove();
  delay(500);

  moveBackward();
  delay(2000);
  stopMove();
  delay(500);

  turnLeft();
  delay(2000);
  stopMove();
  delay(500);

  turnRight();
  delay(2000);
  stopMove();
  delay(500);
}

void moveForward() {
  digitalWrite(A_1B, LOW);        //LOW turns something off
  digitalWrite(A_1A, HIGH);       //HIGH turns something on
  digitalWrite(B_1B, HIGH);  
  digitalWrite(B_1A, LOW);
}

void moveBackward() {
  digitalWrite(A_1B, HIGH);
  digitalWrite(A_1A, LOW);
  digitalWrite(B_1B, LOW);
  digitalWrite(B_1A, HIGH);
}

void turnRight() {
  digitalWrite(A_1B, HIGH);
  digitalWrite(A_1A, LOW);
  digitalWrite(B_1B, HIGH);
  digitalWrite(B_1A, LOW);
}

void turnLeft() {
  digitalWrite(A_1B, LOW);
  digitalWrite(A_1A, HIGH);
  digitalWrite(B_1B, LOW);
  digitalWrite(B_1A, HIGH);
}

void stopMove() {
  digitalWrite(A_1B, LOW);
  digitalWrite(A_1A, LOW);
  digitalWrite(B_1B, LOW);
  digitalWrite(B_1A, LOW);
}
```



# Bill of Materials
Here's where you'll list the parts in your project. To add more rows, just copy and paste the example rows below.
Don't forget to place the link of where to buy each component inside the quotation marks in the corresponding row after href =. Follow the guide [here]([url](https://www.markdownguide.org/extended-syntax/)) to learn how to customize this to your project needs. 

| **Part** | **Note** | **Price** | **Link** |
|:--:|:--:|:--:|:--:|
| Item Name | What the item is used for | $Price | <a href="https://www.amazon.com/Arduino-A000066-ARDUINO-UNO-R3/dp/B008GRTSV6/"> Link </a> |
| Item Name | What the item is used for | $Price | <a href="https://www.amazon.com/Arduino-A000066-ARDUINO-UNO-R3/dp/B008GRTSV6/"> Link </a> |
| Item Name | What the item is used for | $Price | <a href="https://www.amazon.com/Arduino-A000066-ARDUINO-UNO-R3/dp/B008GRTSV6/"> Link </a> |

# Other Resources/Examples
One of the best parts about Github is that you can view how other people set up their own work. Here are some past BSE portfolios that are awesome examples. You can view how they set up their portfolio, and you can view their index.md files to understand how they implemented different portfolio components.
- [Example 1](https://trashytuber.github.io/YimingJiaBlueStamp/)
- [Example 2](https://sviatil0.github.io/Sviatoslav_BSE/)
- [Example 3](https://arneshkumar.github.io/arneshbluestamp/)

To watch the BSE tutorial on how to create a portfolio, click here.
