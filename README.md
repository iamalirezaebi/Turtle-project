# Turtle project
  in this project i simply went through a library in python using it's documentation to get familiar with turtle library
  in order to be more fruitful project i tried to do some challenges;
#### First challenge : draw a square
  in this challenge i realized that i can simply move forward and turn 90 degrees to left or right and repeat the same process
  until the fourth run.
#### Second challenge : draw a dashed line 
  this was a bit more challenging and i found two methods to do this the first one : using pen down and pen up; and the second
  one : using painting white and black one in a row
#### Third challenge: draw triangle, rectangle, .. to six angle!
  and the challenge continues to increase! in this part mathematics comes in the way and i should calculate the angles of each 
  shape to draw them back to back; but witrh 60, 90, 108,.. the project got solved, fortunately!:)
#### Fourth challenge: Generate a Random Walk
  creates a turtle graphics program in Python using the turtle module. The program makes a turtle named "ted"           perform a random walk on the screen, changing colors and directions as it moves. Here is a step-by-step explanation   of what the code does:
  Import Modules:     
  import random
  import turtle
  Set Up Turtle and Screen:
  ted = turtle.Turtle()
  turtle.colormode(255)
  Creates a turtle object named "ted".
  Sets the color mode of the turtle to RGB (with values ranging from 0 to 255).
  Define Variables:
  directions = [0, 90, 180, 270]
  ted.width(5)
  ted.speed("fastest")
  directions is a list containing possible directions (0°, 90°, 180°, and 270°).
  Sets the width of the turtle's pen to 5.
  Sets the speed of the turtle to the fastest setting.
  Define decide_color Function:
      b = random.randint(0, 255)
      color_tuple = (r, g, b)
      return color_tuple
  This function generates a random color by creating a tuple with three random integers (r, g, b) each between 0 and    255.
  Returns the color tuple.
  Define random_walk Function:
  def random_walk(n):
      for _ in range(n):
          ted.color(decide_color())
          ted.forward(20)
          ted.setheading(random.choice(directions))
  This function makes the turtle perform a random walk.
  It takes an integer n as an argument, which specifies the number of steps in the walk.
  In each step:
  The turtle's color is set to a random color using decide_color().
  The turtle moves forward by 20 units.
  The turtle changes its heading to a random direction from the directions list.
  Execute Random Walk:
  random_walk(200)
  Calls the random_walk function with 200 steps.
  Set Up Screen Exit:
#### Fifth challenge: Draw a Spirograph
  This code creates a turtle graphics program in Python using the turtle module. The program makes a turtle named 
 "theresa" draw a spirograph, changing colors as it rotates. Here's a detailed explanation of what the code does:
  Import Modules:
  import random
  import turtle
  Set Up Turtle and Screen:
  theresa = turtle.Turtle()
  turtle.colormode(255)
  theresa.speed("fastest")
  Creates a turtle object named "theresa".
  Sets the color mode of the turtle to RGB (with values ranging from 0 to 255).
  Sets the speed of the turtle to the fastest setting.
  Define decide_color Function:
  def decide_color():
      r = random.randint(0, 255)
      g = random.randint(0, 255)
      b = random.randint(0, 255)
      color_tuple = (r, g, b)
      return color_tuple
  This function generates a random color by creating a tuple with three random integers (r, g, b) each between 0 and 255.
  Returns the color tuple.
  Define draw_spirograph Function:
  def draw_spirograph(size_of_gap):
      for _ in range(int(360 / size_of_gap)):
          theresa.color(decide_color())
          theresa.circle(100)
          theresa.setheading(theresa.heading() + size_of_gap)
  This function makes the turtle draw a spirograph.
  It takes an integer size_of_gap as an argument, which specifies the gap size between each circle.
  The loop runs 360 / size_of_gap times:
  Sets the turtle's color to a random color using decide_color().
  Draws a circle with a radius of 100 units.
  Changes the turtle's heading by adding size_of_gap degrees to the current heading.
  Execute Spirograph Drawing:
  draw_spirograph(5)
  Calls the draw_spirograph function with a gap size of 5 degrees.
