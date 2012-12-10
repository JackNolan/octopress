---
layout: post
title: "First Ruby Motion App"
date: 2012-12-10 17:42
comments: true
categories: 
---


I recently dived into rubymotion head first and since there is a definite lack of quality tutorials out there I decided to outline my first ruby motion project. The goal of the project was simple, say display hello world to the user. My first set was setting up the app delicate. The following code is the very generic setup.

```ruby
def application(application,didFinishLaunchingWithOptions:launchOptions)
    @window = UIWindow.alloc.initWithFrame(UIScreen.mainScreen.bounds)
    @window.rootViewController = HomeController.new
    @window.makeKeyAndVisible
    true
  end
```
This will initialize the window and set the initial controller to the homeController. Then in order for this to work I needed to define the HomeController, so in the controllers/home_controller.rb I define my controller.

```ruby
class HomeController < UIViewController
  def loadView
    self.view = UIView.alloc.init
  end
  def viewDidLoad
  end
end
```
This defines the homecontroller and sets the view local variable. This variable will be used to add UI elements to the view. So next is adding a UILabel to this view using the following code

```ruby
label = UILabel.alloc.initWithFrame([[15,100],[140,70]])
label.text = "helloworld"
view.addSubview(label)
```

This code initializes a new UILabel in the given frame the adds the text to display and finally adds it to the view initialized earlier to be displayed. And thats it! We now have our generic helloworld application next thing to do: put it on the app store and make 1 million dollars.