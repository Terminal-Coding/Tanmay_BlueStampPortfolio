
# Smart Walking Stick


<!---

Replace this text with a brief description (2-3 sentences) of your project. This description should draw the reader in and make them interested in what you've built. You can include what the biggest challenges, takeaways, and triumphs from completing the project were. As you complete your portfolio, remember your audience is less familiar than you are with all that your project entails!

You should comment out all portions of your portfolio that you have not completed yet, as well as any instructions:

-->

| **Engineer** | **School** | **Area of Interest** | **Grade** |
|:--:|:--:|:--:|:--:|
| Tanmay P | Moreland Middle School | Aeronautical Engineering | Upcoming 8th Grader


<img src="Tanmay_P.png" width="50%">

<!---

# Modifications

<iframe width="560" height="315" src="https://www.youtube.com/embed/F7M7imOVGug" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>

For vmy smart walking sticks modifications I did a toggle switch and !¡!¡!¡!¡ . Some challenges and problems I encountered while making this were that, one, there weren't enough grounds, to solve this, I created a splitter which basically splits the grounds powers with the toggle switch and buzzer.  Another problem I encountered was the toggle switch randomly going off, after a bit of searching, I was able to find that the issue was with the how the toggle switch's wire was connected, it was very thin and short, to fix this, I cut a male-male wire and soldered both the wires together so it would connect better.

  
# Final Milestone

**Don't forget to replace the text below with the embedding for your milestone video. Go to Youtube, click Share -> Embed, and copy and paste the code to replace what's below.**

<iframe width="560" height="315" src="https://www.youtube.com/embed/F7M7imOVGug" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>

For your final milestone, explain the outcome of your project. Key details to include are:
- What you've accomplished since your previous milestone
- What your biggest challenges and triumphs were at BSE
- A summary of key topics you learned about
- What you hope to learn in the future after everything you've learned at BSE


# Second Milestone

<iframe width="560" height="315" src="https://www.youtube.com/watch?v=dfMKR5l6gR0" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>

My smart walking stick now has all of its hardware complete. To get here, I had to get drill-trained and make a custom 3D box. I used the drill to drill into the cane as well as the box so that they could be attached. The reason I made this box was so that I could 3D print.

-->

# First Milestone

<iframe width="560" height="315" src="https://www.youtube.com/embed/dfMKR5l6gR0" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>

My smart walking stick's electronics are now finished. There is an ultra-sonic sensor, buzzer, and vibration motor. The motor is connected to a solderable breadboard, which then connects to a male-male wire going to the Aurduino; the buzzer has two female-male wires going directly to the Aurduino; and the Ultra Sonci snesors are connected to a breadboard and four more male-male wires leading to the Aurduino. Soldering the motor connections was my main issue. It took me roughly 30 minutes, and I had to be very precise and couldn't touch other metals or it would cause a short circuit. The next thing I am going to do is get all the electronics inside a box and attach them to a cane.

I used the following code:

```c
#include <Arduino.h>

const int sensorPin = A0;  // Sensor connected to analog pin A0
const int buzzerPin = 9;   // Buzzer connected to digital pin 9

void setup() {
    pinMode(sensorPin, INPUT);
    pinMode(buzzerPin, OUTPUT);
    Serial.begin(9600);
}

void loop() {
    int sensorValue = analogRead(sensorPin);
    Serial.println(sensorValue);

    if (sensorValue > 500) {  // Threshold value for light intensity
        digitalWrite(buzzerPin, HIGH);  // Turn buzzer on
    } else {
        digitalWrite(buzzerPin, LOW);  // Turn buzzer off
    }

    delay(100);  // Delay for stability
}

```

# Starter Project

<iframe width="560" height="315" src="https://www.youtube.com/embed/pzsr6izySn8" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>

My starter project was the RGB Slider. This project included three sliders and three LEDs belonging to red, green, and blue colors. Sliders, when moved, change the color of the LEDs. The slider raises or lowers resistance to drive the amount of energy and power flowing to a circuit. During the development of the project, there were some mishaps—I remember one time when the sliders slid out from the PCB and another time applying way too much solder. Having faced and overcome all those obstacles, I am getting ready to work on my next project—a smart walking stick.

<!---

# Schematics 
Here's where you'll put images of your schematics. [Tinkercad](https://www.tinkercad.com/blog/official-guide-to-tinkercad-circuits) and [Fritzing](https://fritzing.org/learning/) are both great resoruces to create professional schematic diagrams, though BSE recommends Tinkercad becuase it can be done easily and for free in the browser. 

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

-->
