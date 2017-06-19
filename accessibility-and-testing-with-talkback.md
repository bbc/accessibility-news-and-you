---
layout: page
title: Accessibility and Testing with TalkBack
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
0. **Turn TalkBack on**, either by activating the '[Accessibility shortcut](#accessibility-shortcut)' or go to 'Settings', then 'Accessibility', here you can turn 'TalkBack' on. 
1. **Navigate back to Chrome** - 'touch and hold' to select menu items, then double tab to activate. If you need to scroll, swipe up or down with a two or three finger swipe.
2. Select '**Default**' from the '**Local TalkBack**' menu, by swiping up or down, or bring up the menu on the screen by swiping up then right, then navigate by swiping left to right to the '**Default**' option, then double tab to select this option. Note if this is not working, then you do not have focus on the browser window, touch and hold in the browser window then try again.
2. Navigate to the last element in the feature before the feature to be tested, this will ensure you don't miss any visually hidden/off screen text at the beginning of the feature. Then swipe from left to right **through each element** in the feature (if you need to go back, swipe right to left). 
- Is all the content read out and make sense? 
- Is the content read out in a logical order following the visual order? 
- Is any content read out more than once?
- Is any visually hidden/off screen text read out, such as for icons?
- Do images have alt text?
- Are there any empty swipes? e.g. You swipe left to right and you don't hear anything. If so, this maybe a bug.
3. Navigate to the beginning of the page, then Select '**Headings and Landmarks**' from the 'Local TalkBack' menu, then swipe from left to right.
- Are all landmarks read out? Not sure what landmarks are? See [W3C ARIA Landmarks Examples](https://w3c.github.io/aria-practices/examples/landmarks/index.html). Not sure what landmarks the feature should read out? See the accessibility acceptance criteria.
- Are all headings read out and in a logical order? Not sure what headings the feature should read out? You can use a desktop browser tool such as the [Web Developer](https://chrome.google.com/webstore/detail/web-developer/bfbameneiokkgbdmiekhjnmfkcnldhhm) add-on for Chrome or Firefox. (Under ‘Information’ select ‘View Document Outline’ - This will show you the heading structure for the selected page.) 
4. Navigate to the end of the feature before the feature to be tested, then select '**Links**' from the 'Local TalkBack' menu by swiping down, then swipe from left to right. Are all links read out? Is any content that is not a link read out?
5. **ARIA** can be used simply to add landmarks/regions/labels to a page or more advanced usage can help with dynmaic content such as page updates or advanced user interface controls such as tabs. Select '**Default**' from the 'Local TalkBack' menu, then swipe from left to right to move through the feature checking that all ARIA is being acknowledge/read out correctly. See the accessibility acceptance criteria for details on what should be read out. Still not sure what should be acknowledged/read out? Ask an Accessiblity Champion.

## General usage

0. If you are not an advanced user, it is recommended to deactive the **passcode** (if the device has one setup) while using TalkBack. It's also recommended to increase the device **display 'Sleep'** time to minutes rather than seconds, this can be changed under 'Settings', then 'Display'.
1. To quickly access TalkBack, enable the '**<a name="accessibility-shortcut"></a>Accessibility shortcut**' by going to 'Settings', then 'Accessibility', and scroll down to 'Accessibility shortcut', turn this on. You can now turn on TalkBack with 2 simple steps (Note, this functionality is buggy, and may not work on your device):
- Press and hold the power button until you hear a sound or feel a vibration.
- Touch and hold two fingers until you hear audio confirmation.
2. To **unlock the screen**: Swipe two fingers up.

### TalkBack menus

0. Active the '**Global TalkBack**' menu, swipe down then left.
1. Active the '**Local TalkBack**' menu, swipe up then right.

### Text navigation rate

TalkBack lets you control whether text is read to you by **paragraph, a line, a word, or a character at a time**. To set the text navigation rate, tap on the text, then swipe up and down to cycle through the options, then swipe left or right to read the text with the option selected.

### Edit boxes and typing

0. To activate an **edit box**, double tab it, the **keyboard** then becomes available at the bottom of the screen.
1. Explore the keyboard by touching, release you finger when you hear the character you want.
2. Dismiss the keyboard by double tapping the back button.
3. **Move the cursor** by using the volume buttons on the device, up moves the cursor to the beginning, down moves the cursor to the end.
4. The 'Local TalkBack' menu (swipe up then right), will also give you the option to move the cursor under 'Cursor control', you can also **select, copy or paste text** here.

## Test using other supported assistive technology

- [Dragon Naturallyspeaking](accessibility-and-testing-with-dragon)
- [JAWS](accessibility-and-testing-with-jaws)
- [NVDA](accessibility-and-testing-with-nvda)
- [Read&Write](accessibility-and-testing-with-read-and-write)
- [VoiceOver OS (Mac)](accessibility-and-testing-with-voiceover-os)
- [VoiceOver iOS (iPhone/iPad)](accessibility-and-testing-with-voiceover-ios)
- [ZoomText Magnifier/Reader](accessibility-and-testing-with-zoomtext)

## Other pages

- [Accessibility and Supported Assistive Technology](accessibility-and-supported-assistive-technology)