# BlueStamp Self Driving Car
<!--Replace this text with a brief description (2-3 sentences) of your project. This description should draw the reader in and make them interested in what you've built. You can include what the biggest challenges, takeaways, and triumphs from completing the project were. As you complete your portfolio, remember your audience is less familiar than you are with all that your project entails!

You should comment out all portions of your portfolio that you have not completed yet, as well as any instructions:-->
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

### How it works: 
As said in the previous milestone, the IR obstacle avoidance sensors and ultrasonic sensor send a wave or ray in front of it, which bounces off an object is received by the sensor. This allows it to measure the distance between an object and itself. I called upon the trigger and echo pins on the ultrasonic module so I could receive data from the ultrasonic wave it sends. The echo pin was set as an input, meaning it receives the wave, while the trigger pin was set as an output, so it's the side that transmits the wave. As for the IR obstacle avoidance module sensors, I used code to set the pin values of the leftIR and rightIR to 7 and 8. Therefore, I had to wire both sensors to their corresponding pins so the code could go to the correct modules. With these measurements, I was able to have the self driving car follow my hand. As long as it was within 5 inches from the sensor, it would receive the signal, and either move forward or stop. For example, if my hand were too close to the sensor, it wouldn't move, but if my hand stayed approximately 5 inches away from the sensor, it would continue following me. Another feature I added was the remote control. To begin using it, I first added the IR receiver to the breadboard and attatched it to pin 12 and VCC and GND so it would receive the remote controllers infrared signals. When a certain button was pressed, it would either stop, move, speed up, or slow down. 

### Description: 
With the IR obstacle avoidance sensors and the ultrasonic sensor finally attatched and coded, I was able to get it to back away from objects whenever it sensed it. In the previous milestone, I hadn't yet added these sensors, so it would bump into everything when I tried to make it move. Now, I'm able to make it follow my hand, and back away from any obstacles in its way. Additionally, I was able to make the self-driving car use certain sensors and codes whenever the corresponding button was pressed. For example, if I pressed the EQ button on the remote controller, it would automatically switch to folowing my hand instead of following the remote controller which it uses by default. 

### Challenges: 
It was challenging to put together code because I had several lines of code used for different functions on my car, and I had to take pieces out of each code and add it to button functions on the remote controller. Due to the movement codes clashing with one another, the car became confused from all the different directions it was receiving, so it didn't work. 

### Plan for the project: 
My plan for the next milestone would be to make it gesture controlled, as I've always seen people using gesture controlled cars as a kid. I thought it was fascinating how they were able to control the movement of an object like it was an extension of themselves. 

# First Milestone
<iframe width="560" height="315" src="https://www.youtube.com/embed/YdEHZaryFaI?si=4RKEKhnF_nQri2_l" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

### How it works: 
I added different sensors which I would code in the future, such as the ultrasonic sensor, and the IR obstacle avoidance sensors. The ultrasonic sensor transmits an ultrasonic wave through one side which hits an object, eventually receiving the wave through the other side. It uses the amount of time it takes to receive the wave after transmitting it to measure the distance between itself and another object. On the other hand, instead of using an ultrasonic wave, the IR obstacle avoidance sensors use infrared light to measure its distance from an object. It sends an infrared ray which reflects off of an object and comes back to the receiver. If there is no object in front of it, the infrared ray wouldn't reflect off anything and would continue traveling. Additionally, the screw on the top of the sensors can be used to adjust its sensitivity. 

### Description: 
For my first milestone, I started with the acrylic board first, adding motors, then wheels to it so I have a shell to test my code on. Next, I started wiring the car to the Arduino Uno board which would allow code to reach different components. Due to the lack of slots to fit each wire in on my Arduino Uno board, I needed to add a mini breadboard, so I could have each wire function properly. I've been able to connect the 5V and GND pin to the mini breadboard, so I could attach other wires to those pins. So far, I've made it move backward, forwards, and rotate in a constant loop. 

### Challenges: 
A challenge I had was putting the wires together, as I've never really worked with wires before, so I kept on running out of place to put them, and almost made one of my IR obstacle avoidance sensors short circuit. During my first week here, I learned that I could set certain rows for 5V and GND pins by connecting them to the breadboard. As the two rows began filling up with wires, I connected those rows to a different spot on the breadboard, so I have enough space for all my wires. 

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

# Schematics

## Module 1 Schematic
![Second schematics Image](https://github.com/Darryn330/Darryn_BSE_Portfolio/blob/36eb88d8df319386fb23179b37f8a08217f09016/Module%202.png)
![Schematics Image](https://github.com/Darryn330/Darryn_BSE_Portfolio/blob/ddcc68968a56fca457298615dc004e6c84094b03/Module%201%20screenshot.png)
![IR Obstacle Avoidance Module Schematic](https://github.com/Darryn330/Darryn_BSE_Portfolio/blob/01ceee8e1a5722c5cfd2b2f8a822e852ecea0c4d/IR%20Obstacle%20Avoidance%20Module%20schematic.jpg)
![Ultrasonic Module Schematic](https://github.com/Darryn330/Darryn_BSE_Portfolio/blob/034e55c0167eb9afb0b44b15ec4e64b73dbb8159/Ultrasonic%20Schematic.jpg)


# Code
Here's where you'll put your code. The syntax below places it into a block of code. Follow the guide [here]([url](https://www.markdownguide.org/extended-syntax/)) to learn how to customize it to your project needs. 

```c++
void setup() {
  // put your setup code here, to run once:
  Serial.begin(9600);
  Serial.println("Hello World!");
}

void loop() {
  // put your main code here, to run repeatedly:

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
