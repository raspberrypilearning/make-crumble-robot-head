## Finding the servo angles for open and closed

The first thing you need to do is to find at what angle the servo holds the mouth open and closed.

We'll start by making `variables`{:class="crumblevariables"} for 'open' and 'closed'. This is not totally necessary but will help to keep our code clear.

--- task ---

Open the Crumble software and in the `Variables`{:class="crumblevariables"} section, click `Add New Variable`{:class="crumblevariable"}. Name the `variable`{:class="crumblevariables"} as 'open'.

Create another `variable`{:class="crumblevariables"} and name it 'closed'.

![Adding variables](images/servoAngles_addingVariables.png)

--- /task ---

The servo has an angle range of 180°. For many devices this means you can set the servo anyone from 0° to 180° but with Crumble, 0° is the midpoint and you can set your servo from -90° to 90°.

Let's start by checking what position 0° puts our robot mouth at.

--- task ---

Grab a `program start`{:class="crumblebasic"} block and add a `servo A 0 degrees`{:class="crumbleinputoutput"} block from the `Input/Output`{:class="crumbleinputoutput"} block palette.

The example here uses the Crumble 'A' terminal, but if you connected your servo to a different terminal you will need to change the `A`{:class="crumbleinputoutput"} to whatever terminal you used.

To save batteries and in case your code is telling a servo to be in a position it doesn't want to be in, add a delay and turn the servo off.

![Servo A to 0°](images/servoAngles_servoTo0Degrees.png)

Run you code and check what position the robot mouth is in.

--- /task ---

--- no-print ---

![Servo at 0°](images/servoAngles_servoAt0Degrees.gif)

--- /no-print ---

--- print-only ---

![Servo at 0°](images/servoAngles_servoAt0Degrees.png)

--- /print-only ---

It makes sense that with the servo at 0° that the mouth would be half-open but you can see from this example that it doesn't always work out that way. My robot mouth is almost totally closed!

From this we can see that fully closed will only mean a small change in angle but we don't know which direction yet.

--- task ---

Change the angle in the `servo A 0 degrees`{:class="crumbleinputoutput"} block. In my example, adding 10 seems like a good idea. I don't want the mouth to go completely into the robot face so a small change is good.

![Servo A to 10°](images/servoAngles_servoTo0Degrees.png)

Run you code and check what position the robot mouth is in.

--- /task ---