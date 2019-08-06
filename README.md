[![Version](https://img.shields.io/cocoapods/v/HTProgressHUD.svg)](http://cocoapods.org/pods/HTProgressHUD)
[![License](https://img.shields.io/cocoapods/l/HTProgressHUD.svg)](http://cocoapods.org/pods/HTProgressHUD)
[![Platform](https://img.shields.io/cocoapods/p/HTProgressHUD.svg)](http://cocoapods.org/pods/HTProgressHUD)

# HTProgressHUD

**HTProgressHUD** is only a fork of **JTProgressHUD** with a custom loading animation.

**JTProgressHUD** is the new **HUD** designed to show **YOUR** views (eg. UIImageView animations) in the **HUD style** **with one line of code**. You can see many HUDs with easy implementation, but **the idea** is that you want that **easy implementation** with **HUD style** (background that block views below so the user knows that something is processing), but want to **show YOUR** animations/views (could be your app’s animated logo). *By DEFAULT* one animation is also included/built-in.

<h3 align="center">
  <img src="https://github.com/kubatruhlar/JTProgressHUD/blob/master/Screens/builtin.gif" alt=“Builtin”/>
<img src="https://github.com/kubatruhlar/JTProgressHUD/blob/master/Screens/custom.gif" alt=“Custom”/>
</h3>


## Installation
There are two ways to add the **HTProgressHUD** library to your project. Add it as a regular library or install it through **CocoaPods**.

`pod 'HTProgressHUD’`

You may also quick try the example project with

`pod try HTProgressHUD`

**Library requires target iOS 7.0 and above**

> **Works in both - Portrait and Landscape modes**


## Usage and Customization

JTProgressHUD is designed as a **singleton** so you don't have to care about it's instances. Just use class methods `- (void)show` and `- (void)hide` or its variations.

### Simple example:
```objective-c
// Your custom view
[JTProgressHUD showWithView:yourAnimationView];

// Built-in view
[JTProgressHUD show];
```

### Methods:

**View** is your custom view (eg. Animated UIImageView or whatever you want). **Style** is the style of the background. Usually it is the dark color between the view and the rest of the app. **Transition** is showing and hiding transitions. **BackgroundAlpha** is the biggest alpha for the background. *All parameters can be setup separately.*

```objective-c
+ (void)showWithView:style:transition:backgroundAlpha:;
+ (void)show;
+ (void)showWithView:;
+ (void)showWithStyle:;
+ (void)showWithTransition:;
+ (void)showWithBackgroundAlpha:;

+ (void)hide;
+ (void)hideWithTransition:;

+ (BOOL)isVisible;
```

## Author
This library is open-sourced by [Jakub Truhlar](http://kubatruhlar.cz).
**HTProgressHUD** animation created by [Vincenzo Romano](https://www.enzoromano.eu). 

## License
The MIT License (MIT)
Copyright © 2015 Jakub Truhlar
