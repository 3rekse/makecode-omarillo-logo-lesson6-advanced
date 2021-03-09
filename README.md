### @explicitHints true

# Turtle Logo - Lesson #6 - Advanced

## Turtle Logo - Lesson, with variables and sprites #6 @unplugged
**Making the Turtle's do Loops.**

In this lesson you will learn to use loops, to make your code more efficient.
![](https://github.com/Mr-Coxall/makecode-arcade-turtle-logo-lesson6-advanced/raw/main/assets/looping_screenshot.png)

## Step 1
Code your solution below.

```ghost
let myTurtle = turtle.fromSprite(sprites.create(img``, SpriteKind.Player))
myTurtle.moveDirection(TurtleDirection.Forward, 0)
myTurtle.turnDirectionByDegrees(TurtleTurnDirection.Right, 90)
myTurtle.setPenColor(0)
myTurtle.pen(TurtlePenMode.Up)
myTurtle.say("Hello, World!")
for (let index = 0; index < 0; index++) {
}
```