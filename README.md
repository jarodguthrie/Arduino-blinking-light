# Arduino-blinking-light

Arduino Lesson ­ Blinking LED
Allow 1 Hour

Objectives:
● Learn about the basics of computer coding and how we use it in our everyday life
● Write and upload your first sketch—a sketch is a program you upload to your arduino
● Learn to use comments, variables, functions, and loops in your code
● Learn to write an electrical circuit schematic

Overview:
Today we will be exploring the Arduino integrated development environment. We will start by building the ‘blink’ circuit, and writing a simple sketch to control the LED light.
We will then breakdown the code components of your sketch, and discuss the role each line of your code plays in the program.

Key Terms:
● Sketch  = a sketch is the name that Arduino uses for a computer program. It's the unit of code that is uploaded and run on an Arduino board.
● Transistor  =  A transistor is a miniature electronic component that can do two different jobs. It can work either as an  amplifier  or a switch:
○ Amplifier: When it works as an amplifier, it takes in a tiny electric current at one end (an input current) and produces a much bigger electric current (an output current) at the other. In other words, it's a kind of current booster.
○ Switch: Transistors can also work as  switches . A tiny electric current flowing through one part of a transistor can make a much bigger current flow through another part of it. In other words, the small current switches on the larger one.
● Algorithm  = In mathematics and computer science, an algorithm is a self­contained step­by­step set of operations to be performed.
● Comment  = information about the program written for humans clarity, it will not affect the program itself.
● Variable  = information or attributes in your program that change, have a variable value.
● Functions  = things your program can do, it’s functionality. For example, turning an LED on, or reading the temperature.
  
 First Exercise
A school crossing has just been installed outside the front of a busy primary school. The crossing consists of both traffic lights for cars, and a pedestrian crossing signal for students. The project manager, Sally, has asked you to provide a program which switches the traffic light on and off every 3 seconds.

1 ­ Draw the schematic for an electrical circuit to solve this problem, including the following components:
● A Red LED
● A 220 ohm resistor

2 ­ Build your Arduino using the schematic you defined above. The configuration should look something like this:
 
3 ­ Now we need to write the program that turns the red LED on and off in a repeating three second interval. Let’s first define the algorithm for our program:
1. 2. 3. 4. 5. 6.

4 ­ We now need to write a  sketch (a small computer program for the Arduino) to perform the instructions (algorithm) in the form of a computer program. Let’s explore the various components of code that we will need to use to write this program.

5 ­ Have a go writing the entire program yourself, your final code should look something like this:

1   /*
2   # Description:
3   # Turns on an LED on for one second, then off for one second, repeatedly.
4   */
5   int  ledPin = 10;
6   void  setup() {
7       pinMode(ledPin, OUTPUT);
8 }
9   void  loop(){
10    digitalWrite(ledPin,HIGH);
11    delay(3000);
12    digitalWrite(ledPin,LOW);
13    delay(3000);
14    }
15


6 ­ Sally has just let us know that the lights actually need to change every two seconds, not three. Update your program to reflect this change.

