import turtle
from turtle import *
        
def draw_shapes():
        window = turtle.getscreen()
        window.bgcolor("black")

        bob = turtle.Turtle()
        bob.shape("triangle")
        bob.color("orange")
        bob.speed(2)

        bobscounter = 0

        while bobscounter < 3:
                bob.forward(100)
                bob.left(120)
                bobscounter = bobscounter + 1
                
        brad = turtle.Turtle()
        brad.shape("turtle")
        brad.color("green")
        brad.speed(3)

        counter = 0

        while counter < 4:
                brad.forward(100)
                brad.right(90)
                counter = counter + 1
        
        angie = turtle.Turtle()
        angie.shape("arrow")
        angie.color("blue")
        angie.circle(100)

        

        color('purple', 'pink')
        begin_fill()
        while True:
            forward(200)
            left(170)
            if abs(pos()) < 1:
                break

        end_fill()

        forward(100)
        right(90)
        forward(200)

        myTurtle = turtle.Turtle()

        def drawSpiral(myTurtle, lineLen):
            if lineLen > 0:
                myTurtle.color("silver")
                myTurtle.forward(lineLen)
                myTurtle.right(90)
                drawSpiral(myTurtle,lineLen-5)

        drawSpiral(myTurtle,100)
       

        done()

        
                   
        window.exitonclick()
        
draw_shapes()


