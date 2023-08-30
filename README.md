# SNAKE-USING-PY
The game Snakes first appeared in Nokia handsets in the late 90’s and since then it has appeared in various phones somewhere around 400 million.
So the first time any of us might have the played the game was probably on a Nokia 3310!. The Unrivaled predecessor of all the Nokia phones.
I played snakes in a later model too which was Nokia 5200 and sliding phone by the company which was graphical and colorful.This game has occupied a lot of attention from all age groups alike.Hence I planned on bringing this legendary game on my laptop and I did that by creating my Snake game with Python!.

Let me show you how I was able to do it.
Curses provides a independent screen painting and keyboard handling for text based terminals and Random is used for randomly generating objects.
curses.initscr() : returns a window object representing an entire screen,
curses.curs_set(0) :allows to maintain the visibility on the terminal where 0 being invisible,1 being normal,2 being very visible.
curses.newwin(sh,sw,0,0): Return a new window whose left upper corner is at 0,0 and of height and width sh and sw.

Then we create the snake object that has to have a smaller size compared to the windows we defined so divided the value by 4 or 2 by choice.Snake is here a list and we can assume it as x and y coordinates and value for simplicity and understanding.The snake has a head,a body part and a tail.The tail is popped and a space is added with every encounter with food.
Now, we create the the food and this has to be placed in the center of the screen and I chose the ‘Pi’ for food and we need the snake to be traveling in a certain direction here I used right this can be varied with our intent.
Next,We create an infinite loop for the snake where the food i.e ‘Pi’ occurs at random position after every snake and food interaction defined a key for receiving a character here up/down/left/right. And if the snake interacts with the Walls of the windows we described then it means we died close the window and spawn a new snake.
snake[1:] means if the snake is found in itself.
Last part, Is to continue creating food within the boundaries specified of the windows and keep making it appear at random points within the windows and another parameter must be checked if the food appears on the snake then no,create a new food point.
A very basic progam and lets remember the snake is on an X-Y plane for justifying its reaction with the keys involved.

References:
https://www.hmdglobal.com/press/2017-02-27-snake/
https://github.com/engineer-man/youtube/tree/master/015

created a small python based game using packages within python.
The initial idea of the game was to get well versed with python and to implement something in less amount of time.
I came across the code on a youtube channel called "engineering man".
I am presently trying to make the code more concise and hopefully a better version of the same code.
In non conda users I highly recommend installing "curses" package in your python
The python version on which I created is 2.7.x
