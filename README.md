# Social-Media-Sentimenatal-Analysis

In this project project, I used tweets dataset from American GOP debates. In this project, I preprocessed the dataset using NLP toolkits before fitting the processed dataset into three different supervised machine learning algorithms. I was able to reach a valid conclusion based on the results of these models. 

This project is useful for opinon modelling, customeers' feedback analysis etc.

import turtle

def draw_rectangle(width, height):
    """Draws a rectangle and returns its center coordinates."""
    turtle.penup()
    turtle.goto(-width/2, height/2)  # Start at top-left corner
    turtle.pendown()
    
    for _ in range(2):
        turtle.forward(width)
        turtle.right(90)
        turtle.forward(height)
        turtle.right(90)

    return (0, 0)  # The center of the rectangle

def draw_star(size):
    """Draws a five-pointed star centered at the current position."""
    turtle.penup()
    turtle.goto(0, -size / 3)  # Adjust starting position for centering
    turtle.pendown()
    
    turtle.setheading(0)  # Face east
    for _ in range(5):
        turtle.forward(size)
        turtle.right(144)

# Setup turtle
turtle.speed(3)

# Draw rectangle and get its center
rect_width = 300
rect_height = 200
center_x, center_y = draw_rectangle(rect_width, rect_height)

# Move to the center of the rectangle
turtle.penup()
turtle.goto(center_x, center_y)
turtle.pendown()

# Draw the star
draw_star(100)

# Hide the turtle and display the drawing
turtle.hideturtle()
turtle.done()
