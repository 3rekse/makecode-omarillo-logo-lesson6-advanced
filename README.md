### @explicitHints true

# Turtle Logo - Lesson #6

## Turtle Logo - Lesson #6 @unplugged
**Making the Turtle's do Loops.**

In this lesson you will learn to use loops, to make your code more efficient.
![loop](https://github.com/Mr-Coxall/makecode-arcade-turtle-logo-lesson6/raw/main/assets/looping_screenshot.png)

## Step 1
** Follow Along**

Once again, all our programs begin with an ⇢``on start``⇠ block. Then you need to add the **Turtle** using the ⇢``show turtle``⇠ block.
```blocks
turtle.showTurtle()
```

## Step 2
** Follow Along**

You know from previous lessons how to move forwards and then turn.
```blocks
turtle.showTurtle()
turtle.moveTurtleDirection(TurtleDirection.Forward, 25)
turtle.turnTurtleDirectionByDegrees(TurtleTurnDirection.Right, 90)
```

## Step 3
**Try it out**

If I asked you to draw a square, what would you do?

Try out some solutions.
![color](https://github.com/Mr-Coxall/makecode-arcade-turtle-logo-lesson6/raw/main/assets/looping_screenshot.png)

## Step 4
** Follow Along**

Most likely you can up with something like this.
```blocks
turtle.showTurtle()
turtle.moveTurtleDirection(TurtleDirection.Forward, 25)
turtle.turnTurtleDirectionByDegrees(TurtleTurnDirection.Right, 90)
turtle.moveTurtleDirection(TurtleDirection.Forward, 25)
turtle.turnTurtleDirectionByDegrees(TurtleTurnDirection.Right, 90)
turtle.moveTurtleDirection(TurtleDirection.Forward, 25)
turtle.turnTurtleDirectionByDegrees(TurtleTurnDirection.Right, 90)
turtle.moveTurtleDirection(TurtleDirection.Forward, 25)
turtle.turnTurtleDirectionByDegrees(TurtleTurnDirection.Right, 90)
```

## Step 5
** Did you know**

When you look at the previous solution, you will notice that the same 2 block were repeated 4 times. In programming this is **a really bad idea**. Repeating yourself encourages errors in your code and is hard to change things if needed.
```blocks
turtle.moveTurtleDirection(TurtleDirection.Forward, 25)
turtle.pen(TurtlePenMode.Up)
```

## Step 6
** Did you know**

What we do instead is use a new block, the ⇢``repeat 4 times, do``⇠ block. It is under the "Loops" menu. 
```blocks
for (let index = 0; index < 4; index++) {
}
```

## Step 7
** Follow Along**

Notice that there is a space inside the block. You can place other blocks in there. Since it has the number "4", any code blocks inside it will be executed 4 times. You can always change the 4 to whatever number you would like. 
```blocks
turtle.showTurtle()
for (let index = 0; index < 4; index++) {
}
```

## Step 8
** Follow Along**

So you can now take your 2 blocks that repeated 4 times and place them inside the ⇢``repeat 4 times, do``⇠ block. This produces a much simpler and easier to maintain program. 
```blocks
turtle.showTurtle()
for (let index = 0; index < 4; index++) {
    turtle.moveTurtleDirection(TurtleDirection.Forward, 25)
    turtle.turnTurtleDirectionByDegrees(TurtleTurnDirection.Right, 90)
}
```

## Step 9
** Try it Out**

You can use the previous example to draw a circle! If you turn a small amount of degrees many times over, you will eventually end up back where you started. The first 7 blocks just move the **Turtle** to not be in the center of the screen.
```blocks
turtle.showTurtle()
turtle.pen(TurtlePenMode.Up)
turtle.moveTurtleDirection(TurtleDirection.Backward, 7)
turtle.turnTurtleDirectionByDegrees(TurtleTurnDirection.Left, 90)
turtle.moveTurtleDirection(TurtleDirection.Forward, 40)
turtle.turnTurtleDirectionByDegrees(TurtleTurnDirection.Right, 90)
turtle.pen(TurtlePenMode.Down)
turtle.setPenColor(8)
for (let index = 0; index < 120; index++) {
    turtle.moveTurtleDirection(TurtleDirection.Forward, 2)
    turtle.turnTurtleDirectionByDegrees(TurtleTurnDirection.Right, 3)
}
```

## Step 10
**Success!**

You can now use loops, to make your code more efficient.

## Step 11
**Your Turn**

Get your **Turtle** to draw a red octagon (a stop sign). Remember in a regular octagon there 8 sides and all the angles are 45°.
![octagon](https://github.com/Mr-Coxall/makecode-arcade-turtle-logo-lesson6/raw/main/assets/octagon_screenshot.png)

## Step 12
**Done**

You have successfully completed your six lesson in Turtle Logo.

```ghost
turtle.say("Hello, World!")
```
