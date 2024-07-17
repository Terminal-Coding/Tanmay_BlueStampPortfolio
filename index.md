
# Smart Walking Stick


<!---

Replace this text with a brief description (2-3 sentences) of your project. This description should draw the reader in and make them interested in what you've built. You can include what the biggest challenges, takeaways, and triumphs from completing the project were. As you complete your portfolio, remember your audience is less familiar than you are with all that your project entails!

You should comment out all portions of your portfolio that you have not completed yet, as well as any instructions:

-->

| **Engineer** | **School** | **Area of Interest** | **Grade** |
|:--:|:--:|:--:|:--:|
| Tanmay P | Moreland Middle School | Aeronautical Engineering | Upcoming 8th Grader


<img src="Tanmay_P (1).png" width="75%">

<!---

# Modifications

<iframe width="560" height="315" src="https://www.youtube.com/embed/F7M7imOVGug" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>

For my smart walking sticks modifications I did a toggle switch and also added an LED for people to see that someone is there  . Some challenges and problems I encountered while making this were that, one, there weren't enough grounds, to solve this, I created a splitter which basically splits the grounds powers with the toggle switch and buzzer.  Another problem I encountered was the toggle switch randomly going off, after a bit of searching, I was able to find that the issue was with the how the toggle switch's wire was connected, it was very thin and short, to fix this, I cut a male-male wire and soldered both the wires together so it would connect better.

<!--
  
# Final Milestone

<iframe width="560" height="315" src="https://www.youtube.com/embed/F7M7imOVGug" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>
 
For your final milestone, explain the outcome of your project. Key details to include are:
- What you've accomplished since your previous milestone
- What your biggest challenges and triumphs were at BSE
- A summary of key topics you learned about
- What you hope to learn in the future after everything you've learned at BSE

For my final milestone I decided to reprint the box with a clip to prevent tilting, as this was a large problem. I've also put all the electronics inside this new box and have gotten everything to work. My biggest challenges while making this project were my vibration motor pulling itself out and my box rotating or being unstable. The best part when I was making this project was when I got the electronics working, it was so cool to see everything work in synchrony. Some of the most important things I learned while making this project was how to solder, how aurdinos work,, and how breadboards work. I hope to learn how I can use all of this to provide input to a device so that I can make larger things.

-->

  ⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯ 

<img src="Screenshot 2024-07-15 at 3.31.00 PM.png" width="100%">

# Second Milestone

<iframe width="560" height="315" src="https://www.youtube.com/embed/Xn5Wfhhhtow" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>

My smart walking stick now has all of its hardware complete. To get here, I had to get drill-trained and make a custom 3D box. I used the drill to drill into the cane as well as the box so that they could be attached. The reason I made this box was so that I could put all the electronics inside. A challenge that came was finding the right screw for the box to attach to, it took me a lot of time as I needed something very thing as well as decently long. However if it was thin and long it could block the electronics so finding something perfect took a long time. Another challenge was the box tilting to the side, to solve this I added tape, in the future I plan to either add another bolt or hot glue. The next thing I will do is put all the eloctronics in the box and make everything usable. 

<img src="Dazzling Turing.png" width="100%">

# First Milestone

<iframe width="560" height="315" src="https://www.youtube.com/embed/dfMKR5l6gR0" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>

My smart walking stick's electronics are now finished. There is an ultra-sonic sensor, buzzer, and vibration motor. The motor is connected to a solderable breadboard, which then connects to a male-male wire going to the Aurduino; the buzzer has two female-male wires going directly to the Aurduino; and the Ultra Soncic snesors are connected to a breadboard and four more male-male wires leading to the Aurduino. Soldering the motor connections was my main issue. It took me roughly 30 minutes, and I had to be very precise and couldn't touch other metals or it would cause a short circuit. The next thing I am going to do is get a box and attach it to the cane.

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

  ⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯ 

| **Part** | **Note** | **Price** | **Link** |
|:--:|:--:|:--:|:--:|
| Arduino Uno| Controls all inputs and outputs | $27 | <a href="https://www.amazon.com/Arduino-A000066-ARDUINO-UNO-R3/dp/B008GRTSV6/"> Link </a> |
| Buzzer| Provides sound for the user to hear | $0.95 | <a href="https://www.adafruit.com/product/1536?gad_source=1&gclid=CjwKCAjw4ri0BhAvEiwA8oo6Fxwn3jKEl9qArXyle2q9GgFVSOuGYgxT8sPOZ8GS1q-iavJMe7XK8RoCrdsQAvD_BwE/"> Link </a> |
| Vibration motor | Provides vibration for user to feel | $8 | <a href="hhttps://www.amazon.com/uxcell-a11101800ux0165-1100RPM-Speed-Vibration/dp/B0087Y95X4"> Link </a> |
| Cane | For the user to grab and hold | $14 | <a href="https://www.homedepot.com/p/DMI-Deluxe-Adjustable-Foot-Cane-with-Offset-Foam-Grip-in-Black-502-1304-0255/204652972?source=shoppingads&locale=en-US&srsltid=AfmBOorhX83EwS5XUpGJGjpv062Aeth-qALnwaV2xnqj2bhnECprqG07ypU"> Link </a> |
| Toggle Switch| Saves battery and allows device  to be turned on and off (bought in packs of 10) | $8 | <a href="[https://www.amazon.com/Arduino-A000066-ARDUINO-UNO-R3/dp/B008GRTSV6/](https://www.amazon.com/Twidec-Pre-soldered-Wires%EF%BC%88Quality-Assurance-Years%EF%BC%89KCD1-3-101-X/dp/B07SPY9H7Y/ref=asc_df_B07SPY9H7Y/?tag=hyprod-20&linkCode=df0&hvadid=692875362841&hvpos=&hvnetw=g&hvrand=8252835168938717860&hvpone=&hvptwo=&hvqmt=&hvdev=c&hvdvcmdl=&hvlocint=&hvlocphy=9032183&hvtargid=pla-2281435178818&psc=1&mcid=8cd80d0c1e403c4dacfe7c2d4edfcf39&hvocijid=8252835168938717860-B07SPY9H7Y-&hvexpln=73&gad_source=1)"> Link </a> |

  ⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯ 

# Starter Project

<iframe width="560" height="315" src="https://www.youtube.com/embed/pzsr6izySn8" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>

My starter project was the RGB Slider. This project included three sliders and three LEDs belonging to red, green, and blue colors. Sliders, when moved, change the color of the LEDs. The slider raises or lowers resistance to drive the amount of energy and power flowing to a circuit. During the development of the project, there were some mishaps—I remember one time when the sliders slid out from the PCB and another time applying way too much solder. Having faced and overcome all those obstacles, I am getting ready to work on my next project—a smart walking stick.

<!---

# Schematics 
Here's where you'll put images of your schematics. [Tinkercad](https://www.tinkercad.com/blog/official-guide-to-tinkercad-circuits) and [Fritzing](https://fritzing.org/learning/) are both great resoruces to create professional schematic diagrams, though BSE recommends Tinkercad becuase it can be done easily and for free in the browser. 

# Bill of Materials
Here's where you'll list the parts in your project. To add more rows, just copy and paste the example rows below.
Don't forget to place the link of where to buy each component inside the quotation marks in the corresponding row after href =. Follow the guide [here]([url](https://www.markdownguide.org/extended-syntax/)) to learn how to customize this to your project needs. 

<!---

# Other Resources/Examples
One of the best parts about Github is that you can view how other people set up their own work. Here are some past BSE portfolios that are awesome examples. You can view how they set up their portfolio, and you can view their index.md files to understand how they implemented different portfolio components.
- [Example 1](https://trashytuber.github.io/YimingJiaBlueStamp/)
- [Example 2](https://sviatil0.github.io/Sviatoslav_BSE/)
- [Example 3](https://arneshkumar.github.io/arneshbluestamp/)

To watch the BSE tutorial on how to create a portfolio, click here.

-->
