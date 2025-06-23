# Custom Object Detection and Sorting 

<!---Replace this text with a brief description (2-3 sentences) of your project. This description should draw the reader in and make them interested in what you've built. You can include what the biggest challenges, takeaways, and triumphs from completing the project were. As you complete your portfolio, remember your audience is less familiar than you are with all that your project entails!-->

<!---You should comment out all portions of your portfolio that you have not completed yet, as well as any instructions:-->

| **Engineer** | **School** | **Area of Interest** | **Grade** |
|:--:|:--:|:--:|:--:|
| Aaron H | VCHS | Mechanical Engineering | Incoming Sophomore

<!---# !!!!edits needed
**Replace the BlueStamp logo below with an image of yourself and your completed project. Follow the guide [here](https://tomcam.github.io/least-github-pages/adding-images-github-pages-site.html) if you need help.**-->

![Headstone Image](AaronH.jpeg)

<!---# Final Milestone

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


-->
# First Milestone

<iframe width="560" height="315" src="https://www.youtube.com/embed/dWyWQxh6dHo?si=aaolCBvaJNcAtCRP" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!---
For your first milestone, describe what your project is and how you plan to build it. You can include:
- An explanation about the different components of your project and how they will all integrate together
- Technical progress you've made so far
- Challenges you're facing and solving in your future milestones
- What your plan is to complete your project
-->

## Milestone Overview
Setting up the Raspberry Pi and getting it to run a premade TensorFlow Lite model

For this milestone, I set up the Raspberry Pi to be able to be controlled by my computer. I also connected a VNC to the Pi so that I could access the camera and file directories easier. Then, I installed everything required for the Tensorflow Lite model to work, and inserted the model onto the Raspberry Pi. My system now can detect items held up to the camera, including water bottles, laptops, and sweatshirts.

## Technical Progress
### SSH-ing into the Raspberry Pi
When flashing the SD card for the Raspberry Pi, I set the hostname and login for the Raspberry Pi so I could SSH into it. I set up a way to quickly access the Raspberry Pi host without needing to run a complicated set of commands using Visual Studio Code. 

### Setting up the VNC
The VNC lets me access the camera through the command ``` libcamera-hello --timeout 0``` and lets me operate the Pi through PiOS. To set this up, I installed TigerVNC, which lets me SSH onto the Raspberry Pi, but more importantly, lets me view and edit all the files and confirgurations of the Pi easily.

### Installing Dependencies
To run Tensorflow lite, many dependencies need to be installed. These include ``` python3-pip ```, ```python3-setuptools```, ``` python3.11-venv ```, ``` python3-numpy```, ``` python3-pillow```, ``` python3-pygame```, ``` python3-picamera2 ```, ``` festival ```, and many more. 

### Integrating a premade Tensorflow Lite model
To run the Tensorflow Lite model, I ran several lines of commands in order to start up the camera and the interface. I tested it on multiple objects to confirm that it worked, and it did.

## Challenges
The first main challenge that I encountered was an error with this peice of code:
```
cd ~
sudo pip3 install --upgrade adafruit-python-shell
wget https://raw.githubusercontent.com/adafruit/Raspberry-Pi-Installer-Scripts/master/raspi-blinka.py
sudo python3 raspi-blinka.py
```
Whenever it was run, it threw me an error related to not having ```adafruit_shell``` installed. I thought it might have had some issues related to the dimensions that we installed, but when I checked, the dependency was already installed. However, the error still persisted. In the end, I just ignored this error and nothing more came of it. Although unsolved, the milestone was still completed.

The second challenge that I had to address was running this peice of code:
```
cd ~
source env/bin/activate
git clone --depth 1 https://github.com/adafruit/rpi-vision.git
cd rpi-vision
pip3 install -e .
```
The first error it threw me was that the directory ```env/bin/activate``` did not exist, and that was because my directory was named differently. The next error was that ```rpi-vision``` did not exist. This was related to the camera connection itself, because I was also no longer able to ping the camera. However, once I power-cycled the Pi and unconnected and reconnected the camera, the error dissapeared. This then let me install the Tensorflow Lite program.

## Lessons learned
A major lesson that I learned was about virtual environments. Raspberry Pi refuses to install packages and dependences without created a "venv", which acts as a codespace isolated from updates which could potentially harm the code. Oftentimes the code broke because I wasn't in a virtual environment, or was in the wrong one.

Another lesson that I learned was related to directories. The change directory, or ```cd```, lets me change between directories, and ```cd ~```returns me to the root directory. When running the Tensorflow Lite model, I often ran it in the wrong directory, which lead to the terminal thowing me an error.

## Next steps
The next step for my project is to integrate my own Tensorflow Lite model from Teachable Machine onto the Raspberry Pi. This way I can learn how to add my own custom objects to be detected by the Raspberry Pi. I can also improve on the quality of the current model by training it more on the Teachable Machine website.

# Bill of Materials
| **Part** | **Note** | **Price** | **Link** |
|:--:|:--:|:--:|:--:|
| Raspberry Pi 4B | Processing | $64.99 | <a href="https://www.amazon.com/Raspberry-Model-2019-Quad-Bluetooth/dp/B07TC2BK1X/"> Link </a> |
| TPU ML Accelerator | Speeds up ML related processes | $96.99 | <a href="https://www.amazon.com/Google-Coral-Accelerator-coprocessor-Raspberry/dp/B07R53D12W/"> Link </a> |
| Camera and Ribbon Cable | Gathers Visual Data | $6.99 | <a href="https://www.amazon.com/Arducam-Raspberry-Camera-Module-1080P/dp/B012V1HEP4/"> Link </a> |
| 5V Brushless Fan | Active Cooling | $4.99 | <a href="https://www.amazon.com/Easycargo-Raspberry-30x30x7mm-Brushless-30mmx30mmx7mm/dp/B0794TXK2W/"> Link </a> |

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
**1x** Circuit Board -> contains processing and code for Tetris  
**6x** Buttons -> 4 for the D-Pad, 1 for the start button, 1 for the pause button  
**2x** 8x8 LED pixel grids -> for the LED display  
**1x** 3 digit 7-segment display -> monitors the score  
**1x** Capacitor -> stores and maintains working electrical charge  
**1x** Passive Buzzer -> used to make Tetris game sounds  
**1x** Power switch -> toggles power to the circuit board  
**1x** Power switch button cap -> red cap that covers the power switch  
**3x** AAA Battery -> provides power for cicuit board  
**1x** Battery box -> Houses the batteries and directs power to the board with wires  
**10x** screws -> Secures the circuit board and battery box to acrylic  
**4x** Isolation Pillars -> Provides spacing between acrylic and circuit board  
**4x** Copper Pillars -> Provides spacing between acrylic and circuit board  
**2x** Acrylic Main panels -> houses the electrical components  
**4x** Acrylic Side panels -> joins the main panels  

## Challenges faced
The main challenge of this starter project is soldering. The connections were very close to each other, and it was hard to hold the components in place, hold a solder, and hold the solder wire all at once with only two hands, especially as the components kept slipping out from undernes the circuit board as I was trying to solder them. The solder also kept getting dirty and burning the rubber part of the wires, which built up as ash on the solder joints. I had to remove all of those imperfections before my project could work.


