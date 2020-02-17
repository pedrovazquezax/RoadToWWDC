---
layout: post
title:  "Introduction to Playgrounds"
date:   2020-02-19 16:46:37 -0600
categories: playgrounds
author: Yocoyani Ehecatzin Pérez Ayala
---

## What's Playgrounds
Paygrounds is an iPad App where you can learn, experiment and create Swift coding. You have multiple tools and utilities for coding, such as "Hello, Byte", that is a game to learn basic concepts of programming for children and new programmers. To start the tutorial you should download the Playgrounds App.

## Creating your first Playground
If you´re starting to learn programing it's time to know the most important code lines in your life "Hello world". So, let's begin! 

First, open Playgrounds on your iPad, in the bottom of the screen you'll see a section named "More Playgrounds", look for "Blank" playground and select it.

![Image1](https://i.imgur.com/BE55gfO.png)

When you open a new playground you'll see a blank page with a button "Tap to enter code here", if you tap the button you'll be able to start writing, but first we are going to review the most important playground tools.

On the upper left corner you'll find the page icon, if you want to create a new file on your playground that's the place. On the upper right corner you have the "+" symbol you'll find many options to help you with common programming functionalities. And in the bottom right corner running code options are placed, it means that if you want to run your code you have to press the "Run My Code"  button. 

![Image3](https://i.imgur.com/er9IBb4.jpg)

Now that we've seen the basics we can start our programming way. To start you should write the next code:
 ```
print("Hello world")
 ```

* Before running your playground, we should know that "print(*something to print*)" it's the easiest way to display information from our code.

Once you've written the code you could tap run, but you can't see the message yet.

![Image5](https://i.imgur.com/XO92PRD.png)

This is because, when we want to observe a message it's neccesary to clic on  the "abc" square on the right side of the "print()" instruction. If you've selected the square now you got a window with the "Hello world" text.

![Image6](https://i.imgur.com/5JOxoZT.png)

Congratulations! Now you're starting your Swift Programming way.

## A golden ending
To finish this introduction we're going to display a view on Playgrounds. Create a new blank playground and tap to start code writting. Write this lines:

```
import UIKit
import PlaygroundSupport
```

This lines tell Playgrounds to  add UIKit and PlaygroundSupport libraries.
* UIKit is going to help us to work with all the graphic components often used on an iOS App or Mac program.
* PlaygroundSupport it's a library that allows us to display all our components on iPad screen.
Continue writting next lines:

```
let mainView = UIView(frame: CGRect(x: 50.0, y: 50.0, width: 100.0. height: 100.0))
mainView.backgroundColor = .blue
PlaygroundPage.current.liveView = mainView
```
The first line of code configures our main view. We need to specify  the view position, and the size of the view. In the second line we put the background view on blue. And finally we display the view on the screen.

![Image7](https://i.imgur.com/WqRLKsw.png)

Finally, if we want to display another view on the main view we write the next:

 ```
let innerView = UIView(frame: CGRect(x: 50.0, y: 50.0, width: 100.0. height: 100.0))
innerView.backgroundColor = .green
mainView.addSubiew(innerView)
 ```
Here we create another view in the same way as the first one, but at the end line we add our new view on the main view. When we run our code it's more clear the effect.

![Image8](https://i.imgur.com/ptjRn90.png)

Now, it's your turn to experiment with Playgrounds.

 
