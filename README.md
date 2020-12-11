# Recursion-Xmas-Tree

# H A P P Y  H O L I D A Y S ! !

from turtle import *
from shapes import *
from random import randint

myPen = Turtle()
myPen.shape("turtle")
myPen.speed(20)

window = turtle.Screen()
window.bgcolor("#000020")

y = -100
width = 240

#treetrunk
draw_rectangle(myPen, "brown", -15, y-40, 30, 40)

#tree
while width>20:
  width = width - randint(20,30)
  height = randint(15,35)
  x = 0 - width/2
  draw_rectangle(myPen, "green", x, y, width, height)
  y = y + height

#star
draw_star(myPen, "yellow", 4, y, 30)

myPen.penup()
myPen.color("red")
myPen.goto(-190, -170)
myPen.write("Merry Christmas To You, From Jazzmyn!", None, None, "14pt bold")
myPen.hideturtle()  
