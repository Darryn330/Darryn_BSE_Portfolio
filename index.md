# BlueStamp Self Driving Car
Recently, self-driving cars have moved from something we believed would come far later in the future to something we see in our everyday lives. Vehicles such as Waymo have now become much more common in society, taking over the role of drivers. The project below showcases a way to build a self-driving car that allows the user to control it with a device, or have it avoid obstacles in its way. 

```HTML
```

| **Engineer** | **School** | **Area of Interest** | **Grade** |
|:--:|:--:|:--:|:--:|
| Darryn K | Lowell High School | Game Designer | Incoming Freshman

![Headstone Image](https://raw.githubusercontent.com/Darryn330/Darryn_BSE_Portfolio/refs/heads/gh-pages/20250722_160932.jpg)
  
# Final Milestone
<iframe width="560" height="315" src="https://www.youtube.com/embed/jlC7yvA3m10?si=SwYJbej6exJsYQYI" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

### Accomplishments: 
From my previous milestone until now, I've spent several days working on a way to make my car gesture controlled. As a kid, I've always wanted a gesture controlled robot or car that I always saw online, or in stores. After using a remote to make my self-driving car move, I decided to move on to the next milestone which I was really excited to do. I began with making the accelerometer print its x, y, and z coordinates in the serial monitor which I eventually used to send forward, backward, left, and right to my self-driving car's Arduino. Before being able to do this, I had to pair my HC05 bluetooth modules so they could send code to one another. Afterwards, I sent the letters "F, B, L, R, and S" which corresponded to certain movements such as forwards and backwards. The self-driving car received these letters giving me the ability to make an if statement which uses the letters to figure out which way to move. 

### Biggest Challenges And Triumphs:
After finishing my last milestone, everything was going smoothly, until I ran into an issue involving an Arduino Nano. Originally, I was planning to pair the HC05 bluetooth modules together using an Arduino Nano, but it was having a bunch of upload errors, and wouldn't set both the modules to AT-mode. The Bluestamp counselors helped me switch it to another Nano, but that didn't work either, so I just worked on the accelerometer allowing me to save time. Eventually, I used an Arduino Uno to pair the HC05 modules by changing both their baud rates to 38400, but then disaster struck again! The accelerometer I was working on for a while suddenly stopped working, and gave me several error messages. I swapped it several times, but it was useless, none of them gave me the outcome I wanted. Days passed, and I decided to give the accelerometer I started with another chance which led to success! It was giving me error messages the whole time, but now, it randomly started working when I uploaded my code. I felt pretty happy with my work, so after working a little longer the next day, I finally had myself a gesture controlled robot. 

### Summary Of Important Learnings 
During my time at Bluestamp, I learned several things about coding, and engineering. I began without too much knowledge about electrical mechanics, but as I progressed, I learned that there were words like VCC and GND on certain pins which I could use to attatch wires to the correct places. Additionally, I learned that I could use one row on a breadboard for the power pin, ground pin or something else by attatching a wire to that row and putting multiple wires behind it. Without code, a machine would just be a hunk of materials, so it was a crucial part of my project. Overtime, I learned that the programming languages Arduino and Python were pretty similar. Using this, I integrated what I knew about Python to my Arduino code making it a lot easier. Moreover, throughout my time at Bluestamp, I was able to gain a lot of valuable experiences and knowledge which I can utilize in the future. 

### What I Hope To Learn In The Future
In the future, I hope to be able to make my own designs without any help. Seeing movies like Iron Man and Sonic the Hedgehog as a kid led me to have a passion for robots and code. Usually, I play building games that allow me to figure out how things like servos and hinges work. By using ideas from these games and movies, I plan to build myself something small that has several helpful functions in the future. 

## Demo Of The Gesture Controlled Part
<iframe width="560" height="315" src="https://www.youtube.com/embed/rkpsjSegc0k?si=iIy3VLfyVGdtGUoU" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>


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
A challenge I faced was when I accidentally soldered 2 parts together. Due to how close the 2 areas were, the liquidated solder combined, and formed a singular ball. Luckily, there was a device that could suck all the liquid up, so I melted the soldering iron, and used the device. Another problem that occured was that the wires were too long, and the scizzors I had couldn't cut them shorter. Eventually, after a while, I was finally able to cut uneccessary pieces off. 

### Next Steps: 
My next steps are to build the self-driving car, and code it. The project I'm currently doing is the self-driving car, which requires me to build the shell, and code it to avoid obstacles. Building the shell would allow me to have something to test my code in, meaning that I can identify problems in my code, and in the shell. Additionally, I need to add modifications to my car. A few modifications I'm thinking about are to make it gesture controlled, have it jump, or give it a nitro booster. 

# How it works: 

### Overview Of Sensors
I added different sensors such as the ultrasonic sensor and the IR obstacle avoidance sensors. The ultrasonic sensor transmits an ultrasonic wave through one side which hits an object, eventually receiving the wave through the other side. It uses the amount of time it takes to receive the wave after transmitting it to measure the distance between itself and another object. On the other hand, instead of using an ultrasonic wave, the IR obstacle avoidance sensors use infrared light to measure its distance from an object. It sends an infrared ray which reflects off of an object and comes back to the receiver. If there is no object in front of it, the infrared ray wouldn't reflect off anything and would continue traveling. Additionally, the screw on the top of the sensors can be used to adjust its sensitivity. (Refer to schematic 1 for a better idea of how it looks) 

#### Ultrasonic Sensor
As said previously, the IR obstacle avoidance sensors and ultrasonic sensor send a wave or ray in front of it, which bounces off an object is received by the sensor. The ultrasonic sensor has 4 pins named VCC(power), GND(ground), TRIG(trigger), and ECHO. Using wires, I connected TRIG and ECHO to pins 3 and 4 on the Arduino Uno R3 board. I called upon the trigger and echo pins on the ultrasonic module using code so I could receive data from the ultrasonic wave it sends. With the code 'Serial.print' I printed how far the ultrasonic sensor was from another object on a tool called the Serial Monitor which is built into the Arduino IDE coding platform. The echo pin was set as an input, meaning it receives the wave, while the trigger pin was set as an output, so it's the side that transmits the wave. 

#### IR Obstacle Avoidance 
As for the IR obstacle avoidance module sensors, I used code to set the pin values of the leftIR and rightIR to 7 and 8. Each sensor has 3 pins saying VCC(power), GND(ground), and OUT(output). The OUT pin is a digital output signal indicating whether an obstacle is detected or not. Therefore, I had to wire both sensor's OUT pins to their corresponding pins so the code could go to the correct modules. When the 2 sensors detected an object close to it, it made the wheel opposite of it spin backward making it turn away from the object. When both sensors were obstructed, the car moved backwards. 

#### Line Tracking Sensor
The line tracking sensor used infrared light to detect the contrast between the line and the area around it. It shoots out infrared light in front of it and uses the reflected light from the ground to see where the line is. Usually, a darker area would reflect less light, and a lighter background reflects more. Because lines are usually black, they would reflect less light, so the car would know exactly what to follow. 

#### Remote Coontroller
Finally, the last tool I used for my self driving car was a remote control. The remote control uses an IR receiver to receive infrared transmissions from the remote controller. With 21 buttons on it, I was able to set different functions for each button. For example, the fast forward and rewind buttons activated the ultrasonic or IR obstacle avoidance sensors while the numbered buttons allowed me to control the direction it goes. 

#### HC05 Module
The HC05 Module allows devices to communicate with each other via  bluetooth. You can configure it as either a Master or Slave device, the Master HC05 sending the signals to the Slave HC05. After receiving these signals, the Slave HC05 gives it to the microcontroller it's connected to allowing them to communicate efficiently. If you use a delay, the Slave HC05 may react to signals slower because it piles up over time, but the module can't carry out that many commands at the same time. 

#### Accelerometer
The accelerometer allows the user to measure the acceleration of itself when it's moving. Most accelerometers contain a small seismic mass which is suspended by springs or something similar. When accelerating, inertia causes the seismic mass to lag back a bit, causing these springs to stretch or compress, which it then converts into signals which it can send to my Arduino Uno board. 

# Schematics
Schematic 3:
![Third schematics Image](https://raw.githubusercontent.com/Darryn330/Darryn_BSE_Portfolio/refs/heads/gh-pages/Milestone%203.png)

Schematic 2: 
![Second schematics Image](https://raw.githubusercontent.com/Darryn330/Darryn_BSE_Portfolio/refs/heads/gh-pages/Module%202.png)

Schematic 1:
![Schematics Image](https://raw.githubusercontent.com/Darryn330/Darryn_BSE_Portfolio/refs/heads/gh-pages/Module%201%20screenshot.png)

# Code
### Milestone 3 Code
#### Master Module
```c++
#include <SoftwareSerial.h>
#include <Wire.h>
#include <SPI.h>
#include <Adafruit_LSM6DS.h>
#include <Adafruit_Sensor.h>
#include <Adafruit_LIS3DH.h>

// Used for software SPI
#define LIS3DH_CLK 13
#define LIS3DH_MISO 12
#define LIS3DH_MOSI 11
// Used for hardware & software SPI
#define LIS3DH_CS 10

SoftwareSerial Master(2,3);

Adafruit_LIS3DH lis = Adafruit_LIS3DH();

void setup(void) {
  Serial.begin(115200);
  Master.begin(38400);
  pinMode(3, OUTPUT);
  pinMode(2, INPUT);

  while (!Serial) delay(10);                                        // will pause Zero, Leonardo, etc until serial console opens

  Serial.println("LIS3DH test!");

  if (!lis.begin(0x18)) {                                           // if the i2c address is not 0x18, print couldn't start and stop the program otherwise, print "LIS3DH found!"
    Serial.println("Couldnt start");
    while (1) yield();
  }
  Serial.println("LIS3DH found!");

  // lis.setRange(LIS3DH_RANGE_4_G);   

  Serial.print("Range = "); Serial.print(2 << lis.getRange());
  Serial.println("G");

  // lis.setPerformanceMode(LIS3DH_MODE_LOW_POWER);
  Serial.print("Performance mode set to: ");                         //sets the performance mode to the value in lis.getPerformanceMode()
  switch (lis.getPerformanceMode()) {
    case LIS3DH_MODE_NORMAL: Serial.println("Normal 10bit"); break;
    case LIS3DH_MODE_LOW_POWER: Serial.println("Low Power 8bit"); break;
    case LIS3DH_MODE_HIGH_RESOLUTION: Serial.println("High Resolution 12bit"); break; //break stops the code after it happens
  }

  // lis.setDataRate(LIS3DH_DATARATE_50_HZ);
  Serial.print("Data rate set to: ");                                //sets the data rate to the value in lis.getDataRate()
  switch (lis.getDataRate()) {
    case LIS3DH_DATARATE_1_HZ: Serial.println("1 Hz"); break;
    case LIS3DH_DATARATE_10_HZ: Serial.println("10 Hz"); break;
    case LIS3DH_DATARATE_25_HZ: Serial.println("25 Hz"); break;
    case LIS3DH_DATARATE_50_HZ: Serial.println("50 Hz"); break;
    case LIS3DH_DATARATE_100_HZ: Serial.println("100 Hz"); break;
    case LIS3DH_DATARATE_200_HZ: Serial.println("200 Hz"); break;
    case LIS3DH_DATARATE_400_HZ: Serial.println("400 Hz"); break;

    case LIS3DH_DATARATE_POWERDOWN: Serial.println("Powered Down"); break;
    case LIS3DH_DATARATE_LOWPOWER_5KHZ: Serial.println("5 Khz Low Power"); break;
    case LIS3DH_DATARATE_LOWPOWER_1K6HZ: Serial.println("1.6 Khz Low Power"); break;
  }

}

void loop() {
  // lis.read();      // get X Y and Z data at once
  // // Then print out the raw data
  // Serial.print("X:  "); Serial.print(lis.x);
  // Serial.print("  \tY:  "); Serial.print(lis.y);
  // Serial.print("  \tZ:  "); Serial.print(lis.z);

  /* Or....get a new sensor event, normalized */
  sensors_event_t event;
  lis.getEvent(&event); //gives me numbers I need

  /* Display the results (acceleration is measured in m/s^2) */
  Serial.print("\t\tX: "); Serial.print(event.acceleration.x);      //now that I have these numbers, I can use event.acceleration x/y/z
  Serial.print(" \tY: "); Serial.print(event.acceleration.y);
  Serial.print(" \tZ: "); Serial.print(event.acceleration.z);
  Serial.println(" m/s^2 "); 

  Serial.println();

  delay(200);

  if (event.acceleration.x <=-3 && event.acceleration.x >=-10) {     //if event.acceleration.x/y/z is greater than/less than/equal to a certain number, it will use that number to print something and move that direction.
    Serial.println ("Back");
    Master.println ("B");
    delay(200);
  }

  else if (event.acceleration.x >=3 && event.acceleration.x <=10) {
    Serial.println ("Front");
    Master.println ("F");
    delay(200);
  }

  else if (event.acceleration.y <=-3 && event.acceleration.y >=-10)  {
    Serial.println ("Right");
    Master.println ("R");
    delay(200);
  }

  else if (event.acceleration.y >=3 && event.acceleration.y <=10) {
    Serial.println ("Left");
    Master.println ("L");
    delay(200);
  }

  else if (event.acceleration.x <=3 && event.acceleration.x >=-3 && event.acceleration.y <=3 && event.acceleration.y >=-3) {
    Serial.println ("Stop");
    Master.println ("S");
    delay(200);
  }
}
```
#### Slave Module 
```c++
#include <SoftwareSerial.h>

const int A_1B = 5; 
const int A_1A = 6;
const int B_1B = 9;
const int B_1A = 10;

int speed = (150);

SoftwareSerial Slave(11,13);

void setup() {
  pinMode(A_1B, OUTPUT);
  pinMode(A_1A, OUTPUT);
  pinMode(B_1B, OUTPUT);
  pinMode(B_1A, OUTPUT);

  analogWrite(A_1B, 0);
  analogWrite(A_1A, 0);
  analogWrite(B_1B, 0);
  analogWrite(B_1A, 0);

  Serial.begin(38400);
  Slave.begin(38400);
  pinMode(13, OUTPUT);
  pinMode(11, INPUT);
}

void loop () {
  Slave.println("Hello");
  // delay(200);
  if (Slave.available()) {
    String receivedString = Slave.readStringUntil('\n');       // Read until a newline character
    Serial.println("Received: ");
    Serial.println(receivedString);
  }

  String receivedString = Slave.readStringUntil('\n');

  if (receivedString.startsWith ("B")) {                       //if the code from my Master code sends these letters, it will move a certain direction
    moveBackward(speed);
    delay(500);
    stopMove();
  }
  if (receivedString.startsWith("F")) {
    moveForward(speed);
    delay(500);
    stopMove();
  }
  if (receivedString.startsWith ("R")) {
    turnRight(speed); 
    delay(500);
    stopMove();
  }
  if (receivedString.startsWith ("L")) {
    turnLeft(speed); 
    delay(500);
    stopMove();
  }

  if (receivedString.startsWith ("S")) {
    stopMove();
  }
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

```


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

      if (speed >= 255) {                                    //sets max speed to 255
        speed = 255;
      }
      if (speed <= 0) {                                      //sets minimum speed to 0
        speed = 0;
      }
      delay(500);
      stopMove();
    }

    IrReceiver.resume();                                     // Enable receiving of the next value
  }

  int left = digitalRead(leftIR);                            // 0: Obstructed   1: Empty
  int right = digitalRead(rightIR);                          //the numbers above mean that if 0 is printed, there is an obstacle, otherwise, 1 is printed
  
  int speed = 150;

  if (!left && right) {                                      //if left is low, and if the right is empty, it would move to the right
    backLeft(speed);
  } else if (left && !right) {                               //if left is empty and right isn't, move to left
    backRight(speed);
  } else if (!left && !right) {                              //if both are empty, move backward
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


String decodeKeyValue(long result)                             //if a certain button is pressed, it returns what button is pressed, and uses the code for the button
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
const int A_1B = 5;                                       //set motors to certain pins
const int A_1A = 6;
const int B_1B = 9;
const int B_1A = 10;

void setup() {
  pinMode(A_1B, OUTPUT);                                  //set motors as outputs
  pinMode(A_1A, OUTPUT);
  pinMode(B_1B, OUTPUT);
  pinMode(B_1A, OUTPUT);
}

void loop() {                                            //makes it move in this pattern forever
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
  digitalWrite(A_1B, LOW);                            //LOW turns something off
  digitalWrite(A_1A, HIGH);                           //HIGH turns something on
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

| **Part** | **Note** | **Price** | **Link** |
|:--:|:--:|:--:|:--:|
| Sunfounder 3 in 1 kit | This contained all the parts I needed for my self-driving car  | $59.99 | <https://www.amazon.com/SunFounder-Compatible-Tutorials-Including-Controller/dp/B0B778L1DZ/ref=sr_1_1?crid=4P8ENG1Z0VZM&dib=eyJ2IjoiMSJ9.D9LrCZJnua_keVMLJz2FWuuxoH63mAxdEJdYQp8_ZhkffgQav9bKIiDykPzM-DaKg32tmb0-8dQPBeHf3i8n0LSYowfGyGMB8-0o-Y1OZwbH9Oof3n8ehJqtNngzSwWf4cBPpZ6fGnqHkCeovLMeMR75gFAXKC3zARKb_tdvSbQGA6ImIwT6Oc_PbJY-Ptzf3uFJ4Vt0tPYCclF9Qw35EIusUp1j8tFtJXoN6wiJL38.jzz8fJXbpzfY320r3XRqMHQbkOe_oHGwQE6r4AEvqiM&dib_tag=se&keywords=sunfounder+3+in+1+starter+kit+for+arduino+uno+r3&qid=1753302390&sprefix=sunfounder+3+in+1+star%2Caps%2C132&sr=8-1>  |
| LIS3DH Three-Axis Accelerometer | Measuring the tilt of my hand | $4.95 | <https://www.amazon.com/Adafruit-LIS3DH-Triple-Axis-Accelerometer-ADA2809/dp/B01BU70B64> |
| HC05 Bluetooth Module | Connecting the hand-gesture tool I built to my car | $10.39 | <https://www.amazon.com/dp/B071YJG8DR?_encoding=UTF8&psc=1&ref=cm_sw_r_cp_ud_dp_N7DGQW3NX3DNB9EY2T47&ref_=cm_sw_r_cp_ud_dp_N7DGQW3NX3DNB9EY2T47&social_share=cm_sw_r_cp_ud_dp_N7DGQW3NX3DNB9EY2T47> |

# Other Resources/Examples
- [Self Driving car tutorial](https://docs.sunfounder.com/projects/3in1-kit-v2/en/latest/car_project/car_assemble.html)
