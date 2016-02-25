# CS 190 Problem Set #3&mdash;Adding a Second View

Course Home Page: http://physics.stmarys-ca.edu/classes/CS190_S16/index.html.

My St. Mary's Home Page: http://physics.stmarys-ca.edu/lecturers/brianrhill/index.html.

Due: By the beginning of class, Tuesday, March 1st, 2016.

## Reading that is Related to this Week's Lectures and/or This Problem Set

### How Computers Hold Numbers

As you're messing around with the HP-35, you are gaining some insight into how computers hold numbers. Here are two references covering the same material as we covered on Tuesday, February 23rd. The first book has an amusing and enthusiastic style:

* Chapter 1 of the Book "How Computers Do Math":
  * http://bit.ly/HowComputersDoMath

* Section 1.4 of the Book "Digital Design and Computer Architecture":
  * http://bit.ly/HowComputersHoldNumbers

### View Controllers and Segues

This is the material we covered on Thursday, February 25th, and it is the material you need to understand to do this Problem Set. However, Apple's doc can feel pretty advanced, so it would be better to come to office hours than to pound your head against this reading. These references are here for students who want to go farther or who want to know what I read as a refresher when I set up this problem set:

* The "View Controller Programming Guide" has some pretty important but also pretty challenging material:
  * https://developer.apple.com/library/ios/featuredarticles/ViewControllerPGforiPhoneOS/DefiningYourSubclass.html
  * https://developer.apple.com/library/ios/featuredarticles/ViewControllerPGforiPhoneOS/PresentingaViewController.html
  * https://developer.apple.com/library/ios/featuredarticles/ViewControllerPGforiPhoneOS/UsingSegues.html

* Apple's documentation on unwind segues:
  * https://developer.apple.com/library/ios/technotes/tn2298/_index.html

* We also looked at UIImageView, UIImage, and discussed the app wrapper, asset management and app thinning. A wealth of information on subjects like this is the iOS Human Interface Guidelines. Violation of the Guidelines is sometimes checked during the App Store submission process. It is good to not go too far afoul of them if you want your app to get to market quickly.
  * https://developer.apple.com/library/ios/documentation/UserExperience/Conceptual/MobileHIG/index.html

## Directions Specific to this Problem Set

In this problem set, you are going to add a second scene to the storyboard that could show settings or acknowledgements.  Basically you will be retracing exactly what we did in class on Thursday, February 25th. You are well on your way to building apps with multiple scenes if you can do this on your own.

1. (3 pts) Place a button over our original 15-digit display. The four size constraints for this button should cause its edges to exactly line up with the display. Make the button's text the "clear color", so that it doesn't show at all. It will still function even though it is invisible (although there are exceptions to this rule). Actually, for debugging purposes, it might be wise to make the button's text the clear color only once you are confident the button is working, because it is very hard to tell a clear button from a missing or misplaced button.

2. (3 pts) Add a second scene to the view controller. Make the type of the view controller for this scene GaelsViewController. Decorate this scene with a UIImageView and put a UIButton on it. Label the UIButton "DONE".

3. (2 pts) Create a segue that puts the second scene on screen when the transparent button covering the display is pushed.

4. (2 pts) Create an unwind segue that puts our original scene back on screen when the "DONE" button is clicked.

Double-check that your segues work completely. There isn't much point in having storyboard scenes that don't actually come on screen when you click the buttons.

## General Directions for all Problem Sets

1. Fork this repository to create a repository in your own Github account. Then clone your fork to whatever machine you are working on.

2. These problem sets are created with the latest version of Xcode and Mac OS X: XCode 7.2.1 and OS X 10.11.3. Please don't run beta versions of Apple's software. During the term, we might move to Xcode 7.3, depending on Apple's release schedule, the value we perceive in 7.3, and how much burden upgrading would put on IT. Currently Xcode 7.3 is in its third beta and the release notes issues list is pretty long.

3. Under no circumstances copy-and-paste any part of a solution from another student in the class. Also, under no circumstances ask outsiders on Stack Exchange or other programmers' forums to help you create your solution. It is however fine&mdash;especially when you are truly stuck&mdash;to ask others to help you with your solution, provided you do all of the typing. They should only be looking over your shoulder and commenting. It is of course also fine to peruse StackExchange and whatever other resources you find helfpul.

4. Your solution should be clean and exhibit good style. At minimum, Xcode should not flag warnings of any kind. Your style should match Apple's as shown by their examples and declarations. Use the same indentation and spacing around operators as Apple uses. Use their capitalization conventions. Use parts of speech and grammatical number the same way as Apple does.  Use descriptive names for variables. Avoid acronyms or abbreviations. I am still coming up to speed on good Swift style. When there appears to be conflict my style and Apple's, copy Apple's, not mine.

5. When completed, before the class the problem set is due, commit your changes to your fork of the repository. I should be able to simply clone your fork, build it and execute it in my environment without encountering any warnings, adding any dependencies or making any modifications.

###### _The contents of this repository are licensed under the_ [Creative Commons Attribution-ShareAlike License](http://creativecommons.org/licenses/by-sa/3.0/)
