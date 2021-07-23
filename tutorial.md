# Temprature Sensor

## Step 1

Drag the Input on A button pressed and in it put the show string block.
in the show string block drag the join block from the text section.
```blocks
input.onButtonPressed(Button.A, function () {
    basic.showString("Hello" + "World")
})
```

## Step 2

In the first parameter of the join block drag a temprature sensor block from input and in the second parameter of the join block write C
```blocks
input.onButtonPressed(Button.A, function () {
    basic.showString("" + input.lightLevel() + "C")
})
```
## Step 3
Drag another on a ButtonPressed block and click on the a and change it to B. in it again put the join block and in the econd parameter of it write F
```blocks
input.onButtonPressed(Button.B, function () {
    basic.showString("Hello" + "F")
})
```
## Step 4
In the first parameter of the join block put the formula temprature sensor block X 1.8 + 32
```blocks
input.onButtonPressed(Button.B, function () {
    basic.showString("" + (input.lightLevel() * 1.8 + 32) + "F")
})
```
## Step 5
Try it on your micro:bit!
<script src="https://makecode.com/gh-pages-embed.js"></script><script>makeCodeRender("{{ site.makecode.home_url }}", "{{ site.github.owner_name }}/{{ site.github.repository_name }}");</script>