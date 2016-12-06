---
layout: page
title: Accessibility and Testing with ZoomText
---

ZoomText is a screen magnifier which also has screen reader capabilities. ZoomText should be tested with **Internet Explorer**. Test using an actual device if possible. 

Not sure how to use ZoomText? Watch [ZoomText New User Introduction](https://www.youtube.com/watch?v=jqLo_OmpFmU)

## What should I test?
0. Test the feature using magnification
1. Test the feature using magnification and the App Reader 

## Testing steps

The accessibility acceptance criteria can be used for additional manual testing steps on device, this is written by the [Business Analyst](accessibility-news-and-business-analysts) and part of their checklist. 

0. Enable ZoomText (ALT + INS)
1. If speech is on, turn this off (ALT + SHIFT + S)
2. Ensure the magnification power is atleast 2x. Select the 'Magnifier' tab, under 'Zoom Window' use the up and down interface arrows to change the magnification power.
3. Select a window Type (CTRL + SHIFT + Z) and move the cursor around the window/feature in Internet Explorer. Can you easily use and understand the feature? Are you having to scroll large distances for associated content/controls, for example, is the submit button along way from the search input field?
3. Bring up the user interface (ALT + INS) and change the magnification power to 1, then select each of the different 'Colour' schemes in turn, is the feature always fully visible?
5. Does the feature have edit fields, such as a search input? If so, bring up the user interface (ALT + INS), then select each of the different 'Cursor' schemes in turn. Is the cursor enhancement always fully visible in the edit fields?
6. Enable Speech on the Reader (ALT + SHIFT + S). Bring up the user interface (ALT + INS), then select each of the different 'Focus' schemes in turn. Use the tab key on the keyboard to tab through the feature in Internet Explorer (To tab backwards, use SHIFT + TAB). Is your position always indicated on the page? Is the focus ouline clear? Does the focus outline sit on top of text or look irregular? Is content read out correctly? Is any content read out more than once?
7. Bring up the user interface (ALT + INS) and start 'AppRdr' under the 'Reading' tab. Select Internet Explorer and use the mouse to click just before the feature you are testing, it will then start reading, let it read through the feature to the start of the next feature. Is the content read out in a logical order following the visual order? Is content read out correctly? Is any content read out more than once?

## Shortcut keys
* ALT + INS: Enable ZoomText/Display User Interface If Enabled
* ALT + DEL: Disable ZoomText

### Maginifier

#### Increase/Decrease maginification level
* ALT + INS: Enable ZoomText/Bring up the user interface 
* Select the 'Magnifier' tab if this is not selected
* Under 'Zoom Window' use the up and down interface arrows to change the magnification power

#### Window type
* CTRL + SHIFT + Z: Cycle through the different magnification view 'Types', such as full, overlay, lens etc.

### Reader

#### Speech
* ALT + SHIFT + S: Disable/Enable Speech on the Reader

#### App Reader
* Bring up the user interface (ALT + INS)
* Select the 'Reader' tab
* Under 'Reading' select 'AppRdr' (App Reader)
* Select Internet Explorer and use the mouse to click a point for the reader to start reading from
* ENTER will stop/start the reader reading at anytime
* ESC will exit the App Reader

## Test using other supported assistive technology

- [Dragon Naturallyspeaking](assistive-technology-testing-steps-dragon)
- [JAWS](assistive-technology-testing-steps-jaws)
- [NVDA](assistive-technology-testing-steps-nvda)
- [Read and Write](assistive-technology-testing-steps-read-and-write)
- [Talkback](assistive-technology-testing-steps-talkback)
- [VoiceOver OS](assistive-technology-testing-steps-voiceover-os)
- [VoiceOver iOS](assistive-technology-testing-steps-voiceover-ios)

## Other pages

- [Accessibility and Supported Assistive Technology](accessibility-and-supported-assistive-technology)
