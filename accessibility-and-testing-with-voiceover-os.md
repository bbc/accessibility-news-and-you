---
layout: page
title: Accessibility and Testing with VoiceOver Mac OS
---

VoiceOver is the defualt screen reader on **Mac** desktop devices. 

It's recommended to use the **latest OS** that you have access to. Test with **Safari**.

**Not sure how to use VoiceOver**? Watch [Screen Reader Basics: VoiceOver -- A11ycasts](https://www.youtube.com/watch?list=PLNYkxOF6rcICWx0C9LVWWVqvHlYJyqw7g&params=OAFIAVgF&v=5R-6WvAihms&mode=NORMAL&app=desktop) and complete the on device tutorial, go to 'System Preferences', then 'Accessibility', then 'VoiceOver'. Then 'Open VoiceOver Training...'. 

## What should I test?
0. Test the feature by reading every element.
1. Test the feature by reading headers.
2. Test the feature by tabbing through links.
1. Test the feature by reading landmarks.
2. Test the feature for use of ARIA.

## Testing steps

The accessibility acceptance criteria can be used for additional manual testing steps on device, this is written by the [Business Analyst](accessibility-news-and-business-analysts) and part of their checklist.

0. Open **Safari**.
1. Go to the **testing url**.
2. **Turn VoiceOver on**, with shortcut keys 'CMD + F5'. 
3. Navigate to the last element in the feature before the feature to be tested, this will ensure you don't miss any visually hidden/off screen text at the beginning of the feature. Then use 'VO + Right arrow' to read **through each element** in the feature (if you need to go back, 'VO + Left arrow'). 
- Is the all the content read out and make sense? 
- Is the content read out in a logical order following the visual order? 
- Is any content read out more than once?
- Is any visually hidden/off screen text read out, such as for icons?
- Do images have alt text?
- Are there any empty key presses? e.g. You press the keys and you don't hear anything. If so, this maybe a bug.
4. Open the 'Rotor' menu ('VO + U'), then use the 'Right/Left arrow' keys to navigate to the list of '**Headings**', then use the 'Down/Up arrow' keys to read through all the headers in the feature.
- Are all headings read out and in a logical order? Not sure what headings the feature should read out? You can use a desktop browser tool such as the [Web Developer](https://chrome.google.com/webstore/detail/web-developer/bfbameneiokkgbdmiekhjnmfkcnldhhm) add-on for Chrome or Firefox. (Under ‘Information’ select ‘View Document Outline’ - This will show you the heading structure for the selected page.) 
5. Navigate to the end of the feature before the feature to be tested, then use the tab key to read out all '**Links**' in the feature. Are all links read out? Is any content that is not a link read out?
6. Open the 'Rotor' menu ('VO + U'), then use the 'Right/Left arrow' keys to navigate to the list of '**Landmarks**', then use the 'Down/Up arrow' keys to read through all the landmarks in the feature.
- Are all landmarks read out? Not sure what landmarks are? See [W3C ARIA Landmarks Examples](https://w3c.github.io/aria-practices/examples/landmarks/index.html). Not sure what landmarks the feature should read out? See the accessibility acceptance criteria.
7. **ARIA** can be used simply to add landmarks/regions/labels to a page or more advanced usage can help with dynmaic content such as page updates or advanced user interface controls such as tabs. Use 'VO + Right arrow' to move through the feature checking that all ARIA is being acknowledge/read out correctly. See the accessibility acceptance criteria for details on what should be read out. Still not sure what should be acknowledged/read out? Ask an Accessiblity Champion.

## Shortcut keys
You will need to use the **VoiceOver modifier (VO) key ** 'CTRL + OPTION/ALT' in combination with other keys for keyboard shortcuts.

0. **Turn VoiceOver on/off**, either with the shortcut keys 'CMD + F5' or go to 'System Preferences', then 'Accessibility', then 'VoiceOver', here you can 'Enable VoiceOver'. 
1. **Move forwards through every page element**: 'VO + Right arrow'
2. **Move backwards through every page element**: 'VO + Left arrow'
3. Navigate by **forwards through headings**: 'VO + CMD + H'
3. Navigate by **backwards through headings**: 'VO + CMD + H + SHIFT'
4. Navigate **forwards through links**: 'TAB' (When doing this if you do not cycle through all links on the page, go to Safari Preference, then go to 'Advanced' then select 'Press Tab to highlight each item on a webpage')
5. Navigate **backwards through links**: 'TAB + SHIFT'
6. To **activate a link/button**: 'VO + Space bar'
7. Bring up the **Rotor**: 'VO + U'. When the menu is displayed use 'Right/Left arrow' to cycle through the different lists, to cycle through items in a list, use the 'Up/Down arrow'. Press 'Return/Enter' or the Space bar to select an item from a list and close the Rotor menu. Close the Rotor without selecting an item by pressing 'ESC'.
8. To **pause/restart VoiceOver talking**: 'CTRL'
9. Decrease/Increase **speaking rate**: 'VO + CMD + Up/Down arrow'
9. **Interact with an element**: 'VO + SHIFT + Down arrow'. To stop interacting with an element: 'VO + SHIFT + Up arrow'.

Note, sometimes VoiceOver will not scroll the screen when navigating, by moving forward to the next element with 'VO + Right arrow', the page should scroll down to bring this element in view.

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