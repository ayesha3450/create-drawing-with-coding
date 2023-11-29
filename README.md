# create-drawing-with-coding
import turtle
# Function to draw a house
def draw_house(x, y):
    turtle.penup()
    turtle.goto(x, y)
    turtle.pendown()
    
    # Draw the house structure
    for _ in range(4):
        turtle.forward(100)
        turtle.left(90)
    
    # Draw the roof
    turtle.goto(x, y + 100)
    turtle.setheading(45)
    turtle.forward(70)
    turtle.setheading(0)
    turtle.forward(100)
    turtle.setheading(-45)
    turtle.forward(70)
    
    # Draw a door
    turtle.setheading(0)
    turtle.penup()
    turtle.goto(x + 40, y)
    turtle.pendown()
    turtle.setheading(90)
    turtle.forward(40)
    turtle.right(90)
    turtle.forward(20)
    turtle.right(90)
    turtle.forward(40)
    
# Function to draw a tree
def draw_tree(x, y):
    turtle.penup()
    turtle.goto(x, y)
    turtle.pendown()
    
    # Draw the tree trunk
    turtle.color('brown')
    turtle.begin_fill()
    turtle.setheading(90)
    turtle.forward(50)
    turtle.right(90)
    turtle.forward(20)
    turtle.right(90)
    turtle.forward(50)
    turtle.right(90)
    turtle.forward(20)
    turtle.end_fill()
    
    # Draw the tree crown
    turtle.color('green')
    turtle.setheading(90)
    turtle.forward(20)
    turtle.begin_fill()
    turtle.circle(30)
    turtle.end_fill()

# Initialize the Turtle screen
turtle.speed(1)
turtle.bgcolor("sky blue")

# Draw houses and trees
draw_house(-150, -150)
draw_house(50, -150
draw_house(-50, 50)
draw_tree(-170, -120)
draw_tree(120, -120)
draw_tree(-20, 130)

# Hide the turtle and display the drawing
turtle.hideturtle()
turtle.done()
