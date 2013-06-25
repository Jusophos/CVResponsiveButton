# CVResponsiveButton #


## Tags ##

iOS, Objective-C, UIButton, HighlightColor, Delay, Fading, Responsive, xCode

## Overview ##

The CVResponsiveButton class provides the possibility to define a highlight color AND a fading time to get a "responsive" way of touching.

## License ##

The code is licensed under the MIT License.

## Copyright ##

Written by Richard Jung <r.jung@jungit.com>.

## Example ##

Providing an example here:

@[WAITING FOR LINK]

Some example screenshots & a video:

![Sample 1](https://github.com/Jusophos/CVResponsiveButton/raw/master/screenshots/cvresponsivebutton_screenshot_1.png "Sample 1")
![Sample 2](https://github.com/Jusophos/CVResponsiveButton/raw/master/screenshots/cvresponsivebutton_screenshot_2.png "Sample 2")

https://github.com/Jusophos/CVResponsiveButton/raw/master/screenshots/cvresponsivebutton_video.mp4

## Installation ##

Include the following files to your xCode project:

-	CVResponsiveButton.h
-	CVResponsiveButton.m

## Usage ##

You can use the CVResponsiveButton class like the UIButton class, because it is a subclass. As example drag an UIButton instance to interface builder and apply the CVResponsiveButton class.

![Sample 3](https://github.com/Jusophos/CVResponsiveButton/raw/master/screenshots/cvresponsivebutton_screenshot_3.png "Sample 3")

or create it manually

	#import "CVResponsiveButton.h"

	// ...

	CVResponsiveButton *button = [[CVResponsiveButton alloc] initWithFrame:CGRectMake(10, 10, 70, 70)];
	button.highlightBackgroundColor = [UIColor redColor];
	[button setTitle:@"Test" forState:UIControlStateNormal];

	// ...

## Options ##

You have two options

### HighlightBackgroundColor ###

You can set the background color of highlighting state (on touch).

	button.highlightBackgroundColor = [UIColor redColor];

### FadingTime ###

You can set a fading time. It will be the "responsive" time after a touch (fading out). Value in seconds.

	button.fadingTime = 0.7;