---
layout: page
title: Accessibility and Testing with VoiceOver iOS (iPhone/iPad)
---

VoiceOver is the defualt screen reader on iPhone/iPad devices. 

It's recommended to use the **latest OS** that you have access to. Test with **Safari**.

## What should I test?
0. Test the feature by swiping through every element.
1. Test the feature by swiping through headers.
3. Test the feature by swiping through links.
2. Test the feature by swiping through landmarks.
4. Test the feature for use of ARIA.

## Testing steps

The accessibility acceptance criteria can be used for additional manual testing steps on device, this is written by the [Business Analyst](accessibility-news-and-business-analysts) and part of their checklist.

0. Open **Safari**.
1. Go to the **testing url**.
2. **Turn VoiceOver on**, using the '[Accessibility shortcut](#accessibility-shortcut)' or go to 'Settings', then 'General', then 'Accessibility', then 'VoiceOver', here you can turn 'VoiceOver' on.
3. **Navigate back to Safari** - 'Tap' once to select to select items, then double tab to activate the selected item. If you need to scroll, swipe three fingers up or down.
4. Navigate to the last element in the feature before the feature to be tested, this will ensure you don't miss any visually hidden/off screen text at the beginning of the feature. Then swipe from left to right **through each element** in the feature (if you need to go back, swipe right to left). 
- Is all the content read out and make sense? 
- Is the content read out in a logical order following the visual order? 
- Is any content read out more than once?
- Is any visually hidden/off screen text read out, such as for icons?
- Do images have alt text?
- Are there any empty swipes? e.g. You swipe left to right and you don't hear anything. If so, this maybe a bug.
5. Navigate to the end of the feature before the feature to be tested, then select '**Headings**' from the '[Rotor menu](#rotor-menu)', then swipe from top to bottom to read through the headings.
- Are all headings read out and in a logical order? Not sure what headings the feature should read out? You can use a desktop browser tool such as the [Web Developer](https://chrome.google.com/webstore/detail/web-developer/bfbameneiokkgbdmiekhjnmfkcnldhhm) add-on for Chrome or Firefox. (Under ‘Information’ select ‘View Document Outline’ - This will show you the heading structure for the selected page.) 
6. Navigate to the end of the feature before the feature to be tested, then select '**Links**' from the '[Rotor menu](#rotor-menu)', then swipe from top to bottom to read through the links. Are all links read out? Is any content that is not a link read out?
7. Select '**Landmarks**' from the '[Rotor menu](#rotor-menu)' (Note, landmarks are not in the 'Rotor' menu by default, to add landmarks go to 'Settings', then 'General', then 'Accessibility', then 'VoiceOver', then 'Rotor'.), then swipe from top to bottom to read through the landmarks.
- Are all landmarks read out? Not sure what landmarks are? See [W3C ARIA Landmarks Examples](https://w3c.github.io/aria-practices/examples/landmarks/index.html). Not sure what landmarks the feature should read out? See the accessibility acceptance criteria.
8. **ARIA** can be used simply to add landmarks/regions/labels to a page or more advanced usage can help with dynmaic content such as page updates or advanced user interface controls such as tabs. Swipe from left to right to move through the feature checking that all ARIA is being acknowledge/read out correctly. See the accessibility acceptance criteria for details on what should be read out. Still not sure what should be acknowledged/read out? Ask an Accessiblity Champion.

## General usage

0. To quickly access VoiceOver, enable the '**<a name="accessibility-shortcut"></a>Accessibility shortcut**' by going to 'Settings', then 'General', then 'Accessibility', and scroll down to 'Accessibility shortcut', then select 'VoiceOver'. You can now turn on VoiceOver by pressing the 'Home' button 3 times. When VoiceOver is on, pressing the 'Home' button 3 times will turn VoiceOver off.
1. You can navigate by headings, links or landmark etc through the '**<a name="rotor-menu"></a>Rotor menu**'. Rotate two fingers on the screen as if you were turning a dial, to move through the options. Then swipe from top to bottom to read through the option you have selected, such as headings. Note, landmarks are not in the 'Rotor' menu by default, to add landmarks go to 'Settings', then 'General', then 'Accessibility', then 'VoiceOver', then 'Rotor'.

### Speaking rate

If VoiceOver is talking too quick, you can reduce the 'Speaking rate'. Go to 'Settings', then 'General', then 'Accessibility', then 'VoiceOver', here you can adjust the 'Speaking rate'.

## Test using other supported assistive technology

- [Dragon Naturallyspeaking](accessibility-and-testing-with-dragon)
- [JAWS](accessibility-and-testing-with-jaws)
- [NVDA](accessibility-and-testing-with-nvda)
- [Read&Write](accessibility-and-testing-with-read-and-write)
- [TalkBack](accessibility-and-testing-with-talkback)
- [VoiceOver OS (Mac)](accessibility-and-testing-with-voiceover-os)
- [ZoomText Magnifier/Reader](accessibility-and-testing-with-zoomtext)

## Other pages

- [Accessibility and Supported Assistive Technology](accessibility-and-supported-assistive-technology)