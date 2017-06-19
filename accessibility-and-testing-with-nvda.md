---
layout: page
title: Accessibility and Testing with NVDA
---

NVDA is a free screen reader for **PC** desktop devices. 

NVDA should be tested with the latest version of **Firefox**. Test using an actual device if possible.

## What should I test?
0. Test the feature by reading every element.
1. Test the feature by reading headers.
2. Test the feature by tabbing through links.
1. Test the feature by reading landmarks.
2. Test the feature for use of ARIA.

## Testing steps

The accessibility acceptance criteria can be used for additional manual testing steps on device, this is written by the [Business Analyst](accessibility-news-and-business-analysts) and part of their checklist.

0. Open **Firefox**.
1. Go to the **testing url**.
2. **Turn NVDA on**. 
3. Navigate to the last element in the feature before the feature to be tested, this will ensure you don't miss any visually hidden/off screen text at the beginning of the feature. Then use 'Down arrow' to read **through each element** in the feature (if you need to go back, 'Up arrow'). 
- Is all the content read out and make sense? 
- Is the content read out in a logical order following the visual order? 
- Is any content read out more than once?
- Is any visually hidden/off screen text read out, such as for icons?
- Do images have alt text?
- Are there any empty key presses? e.g. You press the keys and you don't hear anything. If so, this maybe a bug.
4. Navigate to the last element in the feature before the feature to be tested, then use 'H' to read **through each heading** in the feature (if you need to go back, 'H + SHIFT'). 
- Are all headings read out and in a logical order? 
- Not sure what headings the feature should read out? You can use a desktop browser tool such as the [Web Developer](https://chrome.google.com/webstore/detail/web-developer/bfbameneiokkgbdmiekhjnmfkcnldhhm) add-on for Chrome or Firefox. (Under ‘Information’ select ‘View Document Outline’ - This will show you the heading structure for the selected page.) 
5. Navigate to the end of the feature before the feature to be tested, then use the 'TAB' key to read out all '**Links**' in the feature (if you need to go back, 'TAB + SHIFT').
- Are all links read out? 
- Is any content that is not a link read out?
6. Navigate to the end of the feature before the feature to be tested, then use 'D' to read through all '**Landmarks**', in the feature (if you need to go back, 'D + SHIFT').
- Are all landmarks read out? 
- Not sure what landmarks are? See [W3C ARIA Landmarks Examples](https://w3c.github.io/aria-practices/examples/landmarks/index.html). Not sure what landmarks the feature should read out? See the accessibility acceptance criteria.
7. **ARIA** can be used simply to add landmarks/regions/labels to a page or more advanced usage can help with dynmaic content such as page updates or advanced user interface controls such as tabs. Use 'Down arrow' to move through the feature checking that all ARIA is being acknowledge/read out correctly. See the accessibility acceptance criteria for details on what should be read out. Still not sure what should be acknowledged/read out? Ask an Accessiblity Champion.

## Shortcut keys

You will need to use the **NVDA modifier key** in combination with other keys for some keyboard shortcuts. The modifier key can be configured, if you are using a laptop it's most likey set to '**CAPS LOCK**'. 

0. **Move forwards through every page element**: 'Down arrow'
1. **Move backwards through every page element**: 'Up arrow'
2. Navigate **forwards through headings**: 'H'
3. Navigate **backwards through headings**: 'H + SHIFT'
4. Navigate **forwards through heading levels**: '1 - 6'
5. Navigate **backwards through heading levels**: '1 - 6 + SHIFT'
6. Navigate **forwards through links**: 'TAB'
7. Navigate **backwards through links**: 'TAB + SHIFT'
8. To **activate a link**: 'Enter'
8. To **activate a button**: 'Enter or Space bar'
9. Navigate **forwards through landmarks**: 'D'
10. Navigate **backwards through landmarks**: 'D + SHIFT'
11. **Stop NVDA talking**: 'CTRL'
12. Toggle **Screen Layout** mode on/off: 'NVDA + V'

For a full list of shortcut keys see [Deque](https://dequeuniversity.com/screenreaders/nvda-keyboard-shortcuts) and [Webaim](http://webaim.org/resources/shortcuts/nvda).

### Screen Layout mode 

The default mode for reading content with NVDA is the 'Screen Layout' mode. This mode reads content in a similar way to how content is displayed on screen. Turning Screen Layout mode off (NVDA + V), displays content in a linear fashion - putting each element on its own line. For example an inline list in Screen Layout mode could be read out all in one go, if Screen Layout mode is off, then each list item will be placed on it's own line and be read individually. Screen Layout mode can be useful for reading tables.

## Test using other supported assistive technology

- [Dragon Naturallyspeaking](accessibility-and-testing-with-dragon)
- [JAWS](accessibility-and-testing-with-jaws)
- [Read&Write](accessibility-and-testing-with-read-and-write)
- [TalkBack](accessibility-and-testing-with-talkback)
- [VoiceOver OS (Mac)](accessibility-and-testing-with-voiceover-os)
- [VoiceOver iOS (iPhone/iPad)](accessibility-and-testing-with-voiceover-ios)
- [ZoomText Magnifier/Reader](accessibility-and-testing-with-zoomtext)

## Other pages

- [Accessibility and Supported Assistive Technology](accessibility-and-supported-assistive-technology)