---
layout: page
title: Accessibility and Testing with Talkback
---

TalkBack is the defualt screen reader on Android devices. 

It's recommended to use the **latest and fastest Android device** you have access to, such as a Nexus 7. Test with **Chrome**.

**Not sure how to use TalkBack**? Complete the on device tutorial, go to 'Settings', then 'Accessibility', then 'TalkBack'. Under TalkBack 'Settings' select 'Launch TalkBack tutorial'. 

## What should I test?
0. Test the feature by swiping through every element.
1. Test the feature by swiping through headers and landmarks.
2. Test the feature by swiping through links.
2. Test the feature for use of ARIA.

## Testing steps

The accessibility acceptance criteria can be used for additional manual testing steps on device, this is written by the [Business Analyst](accessibility-news-and-business-analysts) and part of their checklist.

0. Open **Chrome**.
1. Go to the **testing url**.
0. **Turn TalkBack on**, either by activating the 'Accessibility shortcut' (see notes in General usage below) or go to 'Settings', then 'Accessibility', here you can turn 'TalkBack' on. 
1. **Navigate back to Chrome** - 'touch and hold' to select menu items, then double tab to activate. If you need to scroll, swipe up or down with a two/three finger swipe.
2. Select '**Default**' from the '**Local TalkBack**' menu, by swiping up or down, or bring up this menu on the screen by moving a single finger up then right, then navigate  by swiping left to '**Default*', then double tab to select this option. Note if this is not working, then you do not have focus on the browser window, touch and hold in the browser window then try again.
2. Navigate to the end of the feature before the feature to be tested, this will ensure you don't miss any visually hidden/off screen text at the beginning of the feature. Then swipe from left to right **through each element** in the feature (if you need to go back, swipe right to left). 
- Is the all the content read out and make sense? 
- Is the content read out in a logical order following the visual order? 
- Is any content read out more than once?
- Do icons have off-screen text?
- Do images have alt text?
- Are there any empty swipes?
3. Navigate to the beginning of the page, then Select '**Headings and Landmarks**' from the 'Local TalkBack' menu, then swipe from left to right.
- Are all landmarks read out? Not sure what landmarks the feature should read out? Load the feature in a browser and use Paul J Adam's [Landmarks bookmarklet](http://pauljadam.com/bookmarklets/landmarks.html) to see if the feature uses any Landmarks.
- Are all headings read out and in a logical order? Not sure what headings the feature should read out? You can use a tool such as the [Web Developer](https://chrome.google.com/webstore/detail/web-developer/bfbameneiokkgbdmiekhjnmfkcnldhhm) add-on for Chrome or Firefox. (Under ‘Information’ select ‘View Document Outline’ - This will show you the heading structure for the selected page.) 
4. Navigate to the end of the feature before the feature to be tested, then select '**Links**' from the 'Local TalkBack' menu by swiping down, then swipe from left to right. Are all links read out?
5. If the feature uses dynmaic content such as page updates, dvanced user interface controls such as tabs, or more complex elements such as forms, the page may use **ARIA**. Load the feature in a browser and use Paul J Adam's [ARIA bookmarklet](http://pauljadam.com/bookmarklets/aria.html) to see if the feature uses any ARIA, then check it's being acknowledge/read out correctly by swiping from left to right to move through the feature. Not sure what should be acknowledged/read out? Ask an Accessiblity Champion.

## General usage

0. If you are not an advanced user, it is recommended to deactive the **passcode** (if the device has one setup) while using TalkBack.
1. To quickly access TalkBack, enable the '**Accessibility shortcut**' by going to 'Settings', then 'Accessibility', and scroll down to 'Accessibility shortcut', turn this on. You can now turn on TalkBack with 2 simple steps:
- Press and hold the power button until you hear a sound or feel a vibration.
- Touch and hold two fingers until you hear audio confirmation.
Note, this functionality is buggy, and may not work on your device.
2. To **unlock** the screen: Swipe two fingers up over the lock screen.

### TalkBack menus

0. Active the '**Global TalkBack**' menu, on the screen move a single finger down then left.
1. Active the '**Local TalkBack**' menu, on the screen move a single finger up then right.

### Text navigation rate

TalkBack lets you control whether text is read to you by **paragraph, a line, a word, or a character at a time**. To set the text navigation rate, tap on the text, then swipe up and down to cycle through the options, then swipe left or right to read the text with the option selected.

### Edit boxes and typing

To activate an **edit box**, double tab it, the **keyboard** then becomes available at the bottom of the screen. Explore the keyboard by touching, release you finger when you hear the character you want. You can dismiss the keyboard by tapping the back button. You can move the cursor by using the volume buttons on the device, up moves the cursor to the beginning, down moved the cursor to the end. You can also use the 'Local TalkBack' menu, with the 'Cursor control' option you can move the cursor, select, copy or paste text.

## Test using other supported assistive technology

- [Dragon Naturallyspeaking](accessibility-and-testing-with-dragon)
- [JAWS](accessibility-and-testing-with-jaws)
- [NVDA](accessibility-and-testing-with-nvda)
- [Read&Write](accessibility-and-testing-with-read-and-write)
- [VoiceOver OS](accessibility-and-testing-with-voiceover-os)
- [VoiceOver iOS](accessibility-and-testing-with-voiceover-ios)
- [ZoomText Magnifier/Reader](accessibility-and-testing-with-zoomtext)

## Other pages

- [Accessibility and Supported Assistive Technology](accessibility-and-supported-assistive-technology)