## Finding the servo angles for open and closed

The first thing you need to do is to find at what angle the servo holds the mouth open and closed.

We'll start by making `variables`{:class="crumblevariables"} for 'open' and 'closed'. This is not totally necessary but will help to keep our code clear.

--- task ---

Open the Crumble software and in the `Variables`{:class="crumblevariable"} section, click `Add New Variable`{:class="crumblevariable"}. Name the `variable`{:class="crumblevariable"} as 'open'.

Create another `variable`{:class="crumblevariable"} and name it 'closed'.

![Adding variables](images/servoAngles_addingVariables.png)

--- /task ---

The servo has an angle range of 180°. For many devices this means you can set the servo anyone from 0° to 180° but with Crumble, 0° is the midpoint and you can set your servo from -90° to 90°.

Let's start by checking what position 0° puts our robot mouth at.

--- task ---

Grab a `program start`{:class="crumblebasic"} block and add a 

![Adding variables](images/servoAngles_addingVariables.png)

--- /task ---