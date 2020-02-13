# This is the journal for Comp Sci

1. What did we do?

We tried to make in-depth instructions for making a jelly sandwich.

2. What did you learn?

I learnt that something as simple as making a sandwich can need some very in-depth instructions for a computer.

3. What questions do I have?

What is the simplest way to make instructions for something like fixing a car?

# 2/13/2020

1. What did we do?

Today, we made a dice in python. We changed the colors and made a bargraph for counting the amount of times we got each value.

2. What did you learn?

I learned how to use bargraphs in python. Although I have used the language before I did not know how to create bargraphs.

3. What questions do I have?

How can I make the dice do a simple rotation when I click?

```.py
# These variables are to count the rolls of the dice
ones=0
twos=0
threes=0
fours=0
fives=0
sixes=0

def setup():
    size (600,600)
    background(255)
    
def draw():
    x=0
    delay(1)
    mouseClicked()
    barGraph()
    
def barGraph():
    fill(0)
    textSize(20)
    for x in range(6):
        text(x+1,(50+50*x), 580)
    strokeWeight(5)
    rect(50, 550 - ones, 20, ones)
    stroke(120,120,10)
    rect(100, 550 - twos, 20, twos)
    stroke(0,255,0)
    rect(150, 550 - threes, 20, threes)
    stroke(0,0,255)
    rect(200, 550 - fours, 20, fours)
    stroke(50,50,50)
    rect(250, 550 - fives, 20, fives)
    stroke(25,25,25)
    rect(300, 550 - sixes, 20, sixes)
    stroke(120,120,15)
    
def mouseClicked():
    global ones, twos, threes, fours, fives, sixes
    background(255)
    barGraph()
    fill(255)
    rect(100,100, 400, 400, 10)
    stroke(255,0,0)
    strokeWeight(10)

    
    
    n=random(0,6)
    print(n)
    if 0<=n<1:
        circle(300,300,50)
        ones= ones +1
        print("Number of times one has been rolled ",ones)
    if 1.0<=n<2:
        circle(200,200,50)
        circle(400,400,50)
        twos= twos +1
        print("Number of times two has been rolled ",twos)
    if 2.0<=n<3:
        circle(200,200,50)
        circle(400,400,50)
        circle(300,300,50)
        threes= threes +1
        print("Number of times three has been rolled ",threes)
    if 3.0<=n<4:
        circle(200,200,50)
        circle(400,200,50)
        circle(200,400,50)
        circle(400,400,50)
        fours= fours +1
        print("Number of times four has been rolled ",fours)
    if 4.0<=n<5:
        circle(200,200,50)
        circle(400,200,50)
        circle(200,400,50)
        circle(400,400,50)
        circle(300,300,50)
        fives= fives +1
        print("Number of times five has been rolled ",fives)
    if 5.0<=n<6:
        circle(200,200,50)
        circle(400,200,50)
        circle(200,400,50)
        circle(400,400,50)
        circle(200,300,50)
        circle(400,300,50)
        sixes= sixes +1
        print("Number of times six has been rolled ",sixes)
```
