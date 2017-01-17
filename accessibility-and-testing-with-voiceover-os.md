---
layout: page
title: Accessibility and Testing with VoiceOver OS
---

VoiceOver is the defualt screen reader on Apple **MacBook** devices. 

It's recommended to use the **latest OS** you have access to. Test with **Safari**.

**Not sure how to use VoiceOver**? Watch [Screen Reader Basics: VoiceOver -- A11ycasts](https://www.youtube.com/watch?list=PLNYkxOF6rcICWx0C9LVWWVqvHlYJyqw7g&params=OAFIAVgF&v=5R-6WvAihms&mode=NORMAL&app=desktop) and complete the on device tutorial, go to 'System Preferences', then 'Accessibility', then 'VoiceOver'. Then 'Open VoiceOver Training...'. 

## What should I test?
0. Test the feature by swiping through every element.
1. Test the feature by swiping through headers and landmarks.
2. Test the feature by swiping through links.
2. Test the feature for use of ARIA.

## Testing steps

The accessibility acceptance criteria can be used for additional manual testing steps on device, this is written by the [Business Analyst](accessibility-news-and-business-analysts) and part of their checklist.

0. Open **Safari**.
1. Go to the **testing url**.
0. **Turn VoiceOver on**, with the shortcut keys 'CMD + F5' or go to 'System Preferences', then 'Accessibility', then 'VoiceOver', here you can 'Enable VoiceOver'. 
1. **Navigate back to Chrome** - 'touch and hold' to select menu items, then double tab to activate. If you need to scroll, swipe up or down with a two or three finger swipe.
2. Select '**Default**' from the '**Local TalkBack**' menu, by swiping up or down, or bring up the menu on the screen by swiping up then right, then navigate by swiping left to right to the '**Default**' option, then double tab to select this option. Note if this is not working, then you do not have focus on the browser window, touch and hold in the browser window then try again.
2. Navigate to the last element in the feature before the feature to be tested, this will ensure you don't miss any visually hidden/off screen text at the beginning of the feature. Then swipe from left to right **through each element** in the feature (if you need to go back, swipe right to left). 
- Is the all the content read out and make sense? 
- Is the content read out in a logical order following the visual order? 
- Is any content read out more than once?
- Is any visually hidden/off screen text read out, such as for icons?
- Do images have alt text?
- Are there any empty swipes? If so, this maybe a bug.
3. Navigate to the beginning of the page, then Select '**Headings and Landmarks**' from the 'Local TalkBack' menu, then swipe from left to right.
- Are all landmarks read out? Not sure what landmarks are? See [W3C ARIA Landmarks Examples](https://w3c.github.io/aria-practices/examples/landmarks/index.html). Not sure what landmarks the feature should read out? See the accessibility acceptance criteria.
- Are all headings read out and in a logical order? Not sure what headings the feature should read out? You can use a desktop browser tool such as the [Web Developer](https://chrome.google.com/webstore/detail/web-developer/bfbameneiokkgbdmiekhjnmfkcnldhhm) add-on for Chrome or Firefox. (Under ‘Information’ select ‘View Document Outline’ - This will show you the heading structure for the selected page.) 
4. Navigate to the end of the feature before the feature to be tested, then select '**Links**' from the 'Local TalkBack' menu by swiping down, then swipe from left to right. Are all links read out? Is any content that is not a link read out?
5. **ARIA** can be used simply to add landmarks/regions/labels to a page or more advanced usage can help with dynmaic content such as page updates or advanced user interface controls such as tabs. Select '**Default**' from the 'Local TalkBack' menu, then swipe from left to right to move through the feature checking that all ARIA is being acknowledge/read out correctly. See the accessibility acceptance criteria for details on what should be read out. Still not sure what should be acknowledged/read out? Ask an Accessiblity Champion.

## General usage

0. **Turn VoiceOver on/off**, either with the shortcut keys 'CMD + F5' or go to 'System Preferences', then 'Accessibility', then 'VoiceOver', here you can 'Enable VoiceOver'. 
1. Rotor menu: 'CTRL + ALT + U'. Here you can select different options by using the 'Right/Left arrow key'. You can then navigate the page by the option you have selected such as 'Landmarks' by using the keys 'CTRL + ALT + Up/Down arrow key'. The most useful options are Landmarks, Headings and Links.

### Keyboard shortcuts
You will need to use the VO (VoiceOver) modifier key ('CTRL + OPTION/ALT') in combination with other keys for keyboard shortcuts.

0. To move forwards through every page element: 'CTRL + OPTION/ALT + Right arrow'
1. To move backwards through every page element: 'CTRL + OPTION/ALT + Left arrow'
2. Navigate by headings: 'CTRL + OPTION/ALT + CMD + H'
3. Navigate forwards through links: 'CTRL + OPTION/ALT + TAB'
3. Navigate backwards through links: 'CTRL + OPTION/ALT + TAB + SHIFT'
3. To activate a link/button: 'CTRL + OPTION/ALT + Space bar'
4. To stop VoiceOver talking: 'CTRL'
5. To tell VoiceOver that you want to interact with an element such as a table, or the web page rather than the browser User Interface: 'CTRL + ALT + SHIFT + Down arrow'. To stop interacting with the element: 'CTRL + ALT + SHIFT + Up arrow'.
5. Decrease/Increase speaking rate: 'CTRL + OPTION/ALT + CMD + Up/Down arrow'

Sometimes VoiceOVer will not scoll the screen, 'CTRL + OPTION/ALT + Right arrow', should scroll the page down to the element you are focused on.

## Test using other supported assistive technology

- [Dragon Naturallyspeaking](accessibility-and-testing-with-dragon)
- [JAWS](accessibility-and-testing-with-jaws)
- [NVDA](accessibility-and-testing-with-nvda)
- [Read&Write](accessibility-and-testing-with-read-and-write)
- [Talkback](accessibility-and-testing-with-talkback)
- [VoiceOver iOS](accessibility-and-testing-with-voiceover-ios)
- [ZoomText Magnifier/Reader](accessibility-and-testing-with-zoomtext)

## Other pages

- [Accessibility and Supported Assistive Technology](accessibility-and-supported-assistive-technology)