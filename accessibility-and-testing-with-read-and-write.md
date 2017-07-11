---
layout: page
title: Accessibility and Testing with Read&Write
---

Read&Write is text to speech literacy software which makes the web more accessible for users with dyslexia, reading and other learning difficulties, or anyone whose first language isn't English.

Read&Write **MUST** be tested with **Internet Explorer 11**. If the component/feature is used on a wide range of pages and services, to meet the Definition of Done **Chrome** **SHOULD** also be used for testing (as rendering engines differ greatly between browsers, which may effect how content is read), in order to be considered acceptable for a live release. Test using an actual device if possible.

Not sure how to Read with Read&Write? Watch [Introduction to the Read&Write Gold for PC Reading Toolbar](https://www.youtube.com/watch?v=SUI6WX5-Mmo&t=46s ZoomText New User Introduction) from 4 minutes 6 seconds to 5 minutes 30 seconds.

## What should I test?

0. Test the feature by reading highlighted text elements.
1. Test the feature by reading elements that are hovered over by the mouse.

## Testing steps

The accessibility acceptance criteria can be used for additional manual testing steps on device, this is written by the [Business Analyst](accessibility-news-and-business-analysts) and part of their checklist.

0. Open Read&Write.
1. In the toolbar, under the 'TextHelp' dropdown menu, under 'Current Toolbar' select '**Reading Features**'.
2. In the toolbar, under the 'Play' dropdown menu, make sure **only 'Read by sentence'** is checked. (Ensure 'Automatically read next block of text' and 'Read the web' are not checked).
3. **Use the mouse to highlight** the 1st text element in the feature, then use the 'Play' button in the toolbar, to read the text out. Do this for all the text elements in the feature one by one. Note highlighting maybe difficult if the feature uses '**faux block link**'. This is because the 'faux block link' sits on top of the text which makes highlighting/selecting text difficult.
4. In the toolbar, under the 'Play' dropdown menu, check '**Read the web**', then use the mouse to hover over the different text elements one by one in the feature, the text should be read out. 
5. If the feature uses 'faux block link', you may still have **difficulty** reading many of the text elements. Try hovering over a text elements you can read out, after reading this out, try using the 'Forward' and 'Rewind' buttons in the toolbar, to get to difficult text elements. 
6. If the feature uses 'faux block link', and you are still having difficulty reading many of the text elements. Try checking '**Automatically read next block of text**' in the 'Play' dropdown menu, then use your mouse to hover over the 1st text element in the feature and let it read until the end of the feature, is everything now read out? If not, in the feature before the feature which is being tested, hover over an item which you can read by hovering, then let it read from this element and through the feature which is being tested.
7. Hover over each of the images in the feature, the **alt text** should be read out. Note if the feature uses 'faux block link' you may have difficulty.

Note if using Read&Write 11, you may experience **code in script tags** being read out aswell as **text that is hidden** with CSS, this maybe more noticable when 'Automatically read next block of text' is checked. If these bugs are not present when testing with other assistive technology there is no need to fix them, they are bugs with Read&Write itself (which have been reported to Read&Write).

## Test using other supported assistive technology

- [Dragon Naturallyspeaking](accessibility-and-testing-with-dragon)
- [JAWS](accessibility-and-testing-with-jaws)
- [NVDA](accessibility-and-testing-with-nvda)
- [TalkBack](accessibility-and-testing-with-talkback)
- [VoiceOver OS (Mac)](accessibility-and-testing-with-voiceover-os)
- [VoiceOver iOS (iPhone/iPad)](accessibility-and-testing-with-voiceover-ios)
- [ZoomText Magnifier/Reader](accessibility-and-testing-with-zoomtext)

## Other pages

- [Accessibility and Supported Assistive Technology](accessibility-and-supported-assistive-technology)
