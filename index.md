# !!!!edits needed 
Project Name Needed<br>
Replace this text with a brief description (2-3 sentences) of your project. This description should draw the reader in and make them interested in what you've built. You can include what the biggest challenges, takeaways, and triumphs from completing the project were. As you complete your portfolio, remember your audience is less familiar than you are with all that your project entails!

<!---You should comment out all portions of your portfolio that you have not completed yet, as well as any instructions:-->

```HTML 
<!--- This is an HTML comment in Markdown -->
<!--- Anything between these symbols will not render on the published site -->
```

| **Engineer** | **School** | **Area of Interest** | **Grade** |
|:--:|:--:|:--:|:--:|
| Aaron H | VCHS | Mechanical Engineering | Incoming Sophomore

# !!!!edits needed
**Replace the BlueStamp logo below with an image of yourself and your completed project. Follow the guide [here](https://tomcam.github.io/least-github-pages/adding-images-github-pages-site.html) if you need help.**

![Headstone Image](project)
  
# Final Milestone

# !!!!edits needed
**Don't forget to replace the text below with the embedding for your milestone video. Go to Youtube, click Share -> Embed, and copy and paste the code to replace what's below.**

<iframe width="560" height="315" src="https://www.youtube.com/embed/WIRK_pGdIdA?si=Jmkf0DeEBADPxmr3" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

For your final milestone, explain the outcome of your project. Key details to include are:
- What you've accomplished since your previous milestone
- What your biggest challenges and triumphs were at BSE
- A summary of key topics you learned about
- What you hope to learn in the future after everything you've learned at BSE



# Second Milestone

# !!!!edits needed
**Don't forget to replace the text below with the embedding for your milestone video. Go to Youtube, click Share -> Embed, and copy and paste the code to replace what's below.**

<iframe width="560" height="315" src="https://www.youtube.com/embed/y3VAmNlER5Y" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>

For your second milestone, explain what you've worked on since your previous milestone. You can highlight:
- Technical details of what you've accomplished and how they contribute to the final goal
- What has been surprising about the project so far
- Previous challenges you faced that you overcame
- What needs to be completed before your final milestone 

# First Milestone

# !!!!edits needed
**Don't forget to replace the text below with the embedding for your milestone video. Go to Youtube, click Share -> Embed, and copy and paste the code to replace what's below.**

<iframe width="560" height="315" src="https://www.youtube.com/embed/CaCazFBhYKs" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>

For your first milestone, describe what your project is and how you plan to build it. You can include:
- An explanation about the different components of your project and how they will all integrate together
- Technical progress you've made so far
- Challenges you're facing and solving in your future milestones
- What your plan is to complete your project

# Schematics 
# !!!!edits needed
Here's where you'll put images of your schematics. [Tinkercad](https://www.tinkercad.com/blog/official-guide-to-tinkercad-circuits) and [Fritzing](https://fritzing.org/learning/) are both great resoruces to create professional schematic diagrams, though BSE recommends Tinkercad becuase it can be done easily and for free in the browser. 

# Code
# !!!!edits needed
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
# !!!!edits needed
Here's where you'll list the parts in your project. To add more rows, just copy and paste the example rows below.
Don't forget to place the link of where to buy each component inside the quotation marks in the corresponding row after href =. Follow the guide [here]([url](https://www.markdownguide.org/extended-syntax/)) to learn how to customize this to your project needs. 

| **Part** | **Note** | **Price** | **Link** |
|:--:|:--:|:--:|:--:|
| Item Name | What the item is used for | $Price | <a href="https://www.amazon.com/Arduino-A000066-ARDUINO-UNO-R3/dp/B008GRTSV6/"> Link </a> |
| Item Name | What the item is used for | $Price | <a href="https://www.amazon.com/Arduino-A000066-ARDUINO-UNO-R3/dp/B008GRTSV6/"> Link </a> |
| Item Name | What the item is used for | $Price | <a href="https://www.amazon.com/Arduino-A000066-ARDUINO-UNO-R3/dp/B008GRTSV6/"> Link </a> |

<!---
# Other Resources/Examples
One of the best parts about Github is that you can view how other people set up their own work. Here are some past BSE portfolios that are awesome examples. You can view how they set up their portfolio, and you can view their index.md files to understand how they implemented different portfolio components.
- [Example 1](https://trashytuber.github.io/YimingJiaBlueStamp/)
- [Example 2](https://sviatil0.github.io/Sviatoslav_BSE/)
- [Example 3](https://arneshkumar.github.io/arneshbluestamp/)

To watch the BSE tutorial on how to create a portfolio, click here.
-->

# Starter Project: Retro Arcade Console

<iframe width="560" height="315" src="https://www.youtube.com/embed/WhjaGhmm6Ow?si=g7xkTYvMltJQsVe0" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

## Project Overview

The starter project that I chose is the Retro Arcade Console. When turned on, it starts a pre-coded game of Tetris. The game is run on a 8x16 LED pixel grid, and there is a 3 digit 7-segment display for the score. This project demonstrates how physical input through buttons can translate into electrical signals to play a game. To assemble the console I had to solder all the connections myself, and the project in general was mostly centered around developing my solder skills. I would say that my soldering skills improved a lot, especially when soldering wires very close to each other, where precision is needed to prevent the wires from short-circuiting. 

## Materials Used
1x Circuit Board -> contains processing and code for Tetris
6x Buttons -> 4 for the D-Pad, 1 for the start button, 1 for the pause button
2x 8x8 LED pixel grids -> for the LED display
1x 3 digit 7-segment display -> monitors the score
1x Capacitor -> stores and maintains working electrical charge
1x Passive Buzzer -> used to make Tetris game sounds
1x Power switch -> toggles power to the circuit board
1x Power switch button cap -> red cap that covers the power switch
3x AAA Battery -> provides power for cicuit board
1x Battery box -> Houses the batteries and directs power to the board with wires
10x screws -> Secures the circuit board and battery box to acrylic
4x Isolation Pillars -> Provides spacing between acrylic and circuit board
4x Copper Pillars -> Provides spacing between acrylic and circuit board
2x Acrylic Main panels -> houses the electrical components
4x Acrylic Side panels -> joins the main panels

## Challenges faced
The main challenge of this starter project is soldering. The connections were very close to each other, and it was hard to hold the components in place, hold a solder, and hold the solder wire all at once with only two hands, especially as the components kept slipping out from undernes the circuit board as I was trying to solder them. The solder also kept getting dirty and burning the rubber part of the wires, which built up as ash on the solder joints. I had to remove all of those imperfections before my project could work.


