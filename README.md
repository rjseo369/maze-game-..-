# maze-game-..-
#python
import turtle

t=turtle.Turtle()

t.shape("turtle")

def aaa(x,y):

    for i in range(2): 

        t.up()

        t.goto(x,y)

        if i==0:
            
            t.goto(x,y)

        else:

            t.goto(x-150,y-100)

        t.down()

        t.forward(500)

        t.right(90)

        t.forward(150)

        t.left(90)

        t.forward(500)

        t.up()

        t.goto(x,y-50)

        t.down()

def turn_left():

    t.left(10)

    t.forward(10)

def turn_right():

    t.right(10)

    t.forward(10)
        
s=turtle.Screen()

s.onkey(turn_left, "Left")

s.onkey(turn_right, "Right")

aaa(-300,0)

s.listen()

s.mainloop()
