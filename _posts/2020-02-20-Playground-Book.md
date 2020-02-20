---
layout: post
title:  "Playground Book Introduction"
date:   2020-02-20 13:05:37 -0600
categories: PlaygroundBook
author: Pedro Antonio Vázquez Rodríguez
---
## What is Playground Book?

A playground allows us to learn new concepts through programming. The advantages of learning in a playground is that we can experience, play and create while we learn.


## What do we need to build a Playground bBook?
1. You´ll need a [Free apple Developer Acount](https://developer.apple.com).

2. To build your own Blaygorund Book you will need [Xcode 11.1](https://developer.apple.com/download/more/?name=Xcode%2011.1).

3. Also you will need the [Swift Playgrounds Author Template](https://developer.apple.com/download/more/?=Swift%20Playgrounds%20Author%20Template).

4. The **Playgrounds** App for [Mac](https://apps.apple.com/app/id1496833156) or [iPad](https://apps.apple.com/app/id908519492) to test your playground.

## Setting up your Playground

Open the **Swift Playgrounds Author Template**, we will make a few changes to personalize it.

You need to open the **BuildSettings.xcconfig** file, you can find it on the config files directory.


Here you'll find:

*  The **BUNDLE_IDENTIFIER_PREFIX** is used to  set your team, like in a normal app.
    
          example: com.example

* The **PLAYGROUND_BOOK_FILE_NAME** here you´ll set the Playground Book name.


* The **PLAYGROUND_BOOK_CONTENT_VERSION** here you can set in which version of the playground you are deploying actually.
  
Then you´ll need to open the **ManifestPlist.strings** file, which is located at the _PrivateResources_ group in the _PlaygroundBook_ group.

Here you can modify  the values of the:

* Playground Book Name.

* Chapters Name: you can change or add new chapters.

* Chapters Page Names: here you can change the page names and add new page names.