# Common Code Base

## Overview

The common files which are used commonly in overall application are in this module.

### App Version Check

This file let you check the current version of iOS and upgrade to the latest version of the application.

### API Manager

This file contains API calling methods, which internally calls API and passes the result to the methods defined by the calling class.

### Rechability

This file checks the internet connectivity and let the user know about his internet connection, if it is not connected.

### Notification View

This view is used to show messages / errors in the application.

### PhoneNumberFormatter

This is formatter for PhoneNumber which is generally called to format Phone numbers in the proper manner.

### LoadingView

It is a simple loading view which informs the user that something is happening in the background and he has to wait for some time.

### Animation

This file animate the view whie showing and dismissing.

### ApplicationData

This class maintaing the data throughout the application. It is just like a singleton class which persists data throughout the application.

### Utility

This class is used to write some common methods which can be called by any other class. For e.g. getting navigation bar title label, convert number to currency, convert currency to number, etc.

### Fonts

This class is used to keep same fonts through out the application.

### Constants

This class is used to declare / define constants that can be used throughout the application.

### Colors

This class is used to keep same colors through out the application.


## Code Base

Code for above classes resides in following classes / screens:

### App Version Check

* VersionCheck

### API Manager

* APIManager

### Rechability

* Reachability

### Notification View

* Toast+UIView

### PhoneNumberFormatter

* ECPhoneNumberFormatter

### LoadingView

* LoadingView

### Animation

* UIWindow+Animation

### ApplicationData

* AppData

### Utility

* LTUtility

### Fonts

* UIFont+LTFonts

### Constants

* LTConstants

### Colors

* UIColor+LTColors


* * *

© 2014 V2solutions. All rights reserved.