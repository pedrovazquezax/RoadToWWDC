---
layout: post
title:  "Playground Book Introduction"
date:   2020-02-20 13:05:37 -0600
categories: PlaygroundBook
author: Pedro Antonio Vázquez Rodríguez
---
## What is Playgorund Book?

......
Un playground nos permite aprender conceptos nuevos a través de la programación. Las ventajas de aprender en un playgrounds es que podemos experimentar, jugar y crear mientras aprendemos.

......


## What we need to build a playground book?
1. You´ll need a [Free apple Developer Acount](https://developer.apple.com).

2. To build your own playgorund book you will need [Xcode 11.1](https://developer.apple.com/download/more/?name=Xcode%2011.1).

3. Also you will need the [Swift Playgrounds Author Template](https://developer.apple.com/download/more/?=Swift%20Playgrounds%20Author%20Template).

4. The **Playgrounds** App for [Mac](https://apps.apple.com/app/id1496833156) or [iPad](https://apps.apple.com/app/id908519492) to test your playground.

## Setting up your Playground

Open the **Swift Playgrouns Author Template**, we will make a few changes to personalize it.

You need to open the **BuildSettings.xcconfig** file, you can fin it on the config files directory.


Here you'll find:

*  The **BUNDLE_IDENTIFIER_PREFIX** is used to  set your team, like in a normal app example: com.example

* The **PLAYGROUND_BOOK_FILE_NAME** here you´ll set the Playground Book name.


* The **PLAYGROUND_BOOK_CONTENT_VERSION** here you can set in which version of the playground you are deplyplent actualy.
  
Then you´ll need to open the **ManifestPlist.strings** file, wich is located at the _PrivateResources_ group in the _PlaygroundBook_ group.

Here you can modify  the values of the:

* Playground Book Name.

* Chapters Name: you can change or add new chapters.

* Chapters Page Names: here you can change the pages names and add new pages names.