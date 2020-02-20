---
layout: post
title:  "Data Entry"
date:   2020-02-19 20:07:37 -0600
categories: playgrounds
author: Yocoyani Ehecatzin Pérez Ayala
---
Usually when you create an App or a program, your need to interact with the user, to do it you have to create entries to receive user information. In this post we’re going to create a basic Entry for a view in Playgrounds.

First, we’re going to display a common view. Let’s go to code!!

    import UIKit
    import PlaygroundSupport
    
    class JFTextFeld: UIViewController, UITextFieldDelegate{
	    
	    var textField: UITextField!
	    var label: UILabel!
    
    }
Now we’re creating a **class** named  *JFTextfield* that is a child class of UIViewController and UITextFieldDelegate. Maybe this word a kind of strange if you’re a beginner programmer. So, we need to define some concepts before continue.

* **Class** - When we talk about classes we’re refering to a programming structure where we could storage information from different kind of data and add functionalities. It’s a little bit confuse but in simple word we could define a class as an object template that shows the basic properties of the object.
*  **Inheritance**  -One of the basic features of classes is inheritance, when we have a class, very often it takes properties from a **base class**, because of this the new class is known as a **child class** and it means that inherit qualities from his father. Obviously , a base class hasn’t inheritance from another class.

So, we can explain that *JFTextField* is going to be a view when we could find a text field (UITextField) and a label (UILabel).

Now we should write next code into the class:

    override func loadView(){
	    let view = UIView(frame: CGRect(x: 50.0, y: 50.0, width: 100.0, height: 100.0))
	    view.backgroundColor = .cyan
	    
	    textField.textColor = .black
	    textField.backgroundColor = .white
	    view.addSubview(textField)
	    
	    label = UILabel(frame: CGRect(x: 5, y: 25, width: 100, height: 15))
	    label.backgroundColor = .brown
	    label.textColor = .white
	    view.addSubview(label)
	    self.view = view
	 }
	    
We’ve just created a view to display  a text field and a label.
Now, we need to recieve the the entry from the user on the text field and write it on the label.

Add the following code after our last line on lastView():

    textField.addTarget(self., action: #selector(updateText), for: UIControl.editingChanged)
This line indicates that the text field is waiting to be edit, and when someone changed it’s content you could call the updateText function.

It’s time to write the updateText() function:

    @objc func updateText(){
		    self.label.text = textField.text
	    }
	 
Finally, we have to display our view:

    PlaygroundPage.current.liveView = JFTextFieldController()

You’d see this result:

![Image](https://i.imgur.com/ijsOqh6.jpg)

