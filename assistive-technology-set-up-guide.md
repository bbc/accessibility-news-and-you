---
layout: page
title: Testing with a Screen Reader
---
**Note this page is a work in progress and is not yet complete**.

## Approach

### Mobile

70% of screen reader users use VoiceOver, 20% Talkback

- **Test primarily on Voiceover with Safari** (Not Chrome)
- You should test with Talkback however, you only need to test primarily with Talkback if you are testing an Android App (if time is short just test on Voiceover if it’s HTML). Talkback on Android is flaky with HTML (though it’s getting better) - If testing with Talkback use Firefox or Chrome (though Firefox is best).


### Tablet

Same as above, just test on VoiceOver with Safari for a website.

### Touch devices

Don’t assume people don’t have keyboards for mobile and tablet devices, some people do use bluetooth keyboards with their device as this is easier than using the on screen keyboard if you are visually impaired or standard users making notes in a meeting etc. So tabbing etc. does need to work.

### Desktop PC

- Use IE with Jaws or Firefox with NDVA for testing (Don’t test with Chrome)
- NVDA/Firefox is great for testing, though you also need to test with Jaws/IE before releasing a product as they have a higher number of users (though this is falling)
- Test using the latest version of a screen reader (NVDA users will update, Jaws users don’t update very often as it is expensive (£1k) - however you can just test in the latest version unless there are specific requirements)

Test using both NVDA/Firefox and Jaws/IE if thoroughly testing e.g. a new feature, advanced feature with ARIA.

### Desktop Mac

- Use VoiceOver with Safari (don’t use Chrome for testing)
- Just test in the latest version, no need to test old versions as users will update


## Screen reader installation and basic usage instructions

If you haven’t used a screen reader before or know little about Accessibility you may find it useful to complete the Web Accessibility Online Training course. This is a 2 hour course covering the basics of accessibility, who it is for and accessible web development. This will provide a foundation for what you need to know. http://academy.gateway.bbc.co.uk/Courses/WebAccessibility/ <small>(internal BBC link)</small>

There is also a Screen Reader Testing course available at the Academy.

(More advanced screen reader instructions can be found online)

### VoiceOver Apple Mobile/Tablet

- This comes installed on Apple devices by default
- Turn on by going to ‘Settings’ and looking in ‘General’ for ‘Accessibility’, scroll to the bottom and you should see ‘Accessibility Shortcut’, turn this on, you can now easily turn VoiceOver on and off by triple-clicking the home button at anytime.

**Basic usage:**

When first starting out you may find it easier to load the web page you are testing before triple clicking to turn the screen reader on.
- Double tap screen to activate a menu or the keyboard etc.
- Swipe left or right to go through items on a webpage
- Rotor menu - Put your thumb/finger on the screen, place your index/next finger above this and drag for half a circle clockwise, by doing this you can select what to navigate to when you swipe down or up, headings and links are most useful when surfing a web page.
- You can also place your finger on the screen and move it around to read out the items
- Use 3 fingers to scroll

### VoiceOver Desktop Mac (Safari)
- This comes installed on Mac’s by default

- Use the keyboard shortcut to turn this on and off easily ‘cmd + F5’

**Basic usage:**
- Use the tab key (and ‘tab + shift’ to go backwards) to tab through links
- Use a combination of the left and right arrow key with ‘ctrl + alt’ to read items out between links
- Rotor menu 'ctrl + alt + u' - then use the arrow keys to select items e.g. headings, landmarks etc.

**Keyboard shortcuts:**
- See this great page for keyboard shortcuts for VoiceOver commands: http://help.apple.com/voiceover/vo/en/VOKeysColor_1.html

### Jaws - PC

If you only have a Mac install the Jaws demo version (32bit) on a Virtual Machine (see notes below to install VM):
http://tinyurl.com/l7gmyu

- You are not officially suppose to use the demo version, though you can...
- The demo version will only operate for 40 minutes, you then need to restart Windows (Teams could buy a full version which you could keep on a dongle to swap between testers)

**Basic usage:**
- Use the tab key (and ‘tab + shift’ to go backwards) to read out links
- Use the up and down arrow keys to read out items in between links
- The left arrow key will make the screen reader stop what it is reading
- It may say ‘blank’ between html elements, don’t worry about this, it just thinks there is a line space or something like that
- ‘fn + 1’ will find and read the h1 on the web page
- ‘fn + 2’ will find and read the h2’s within the h1
- ‘fn + 3’ will find and read the h3’s under the previous h2

### NVDA - PC

If you only have a Mac install NVDA on a Virtual Machine (see notes below to install VM):
http://www.nvaccess.org/download/

**Basic usage:**
- Use the tab key (and ‘tab + shift’ to go backwards) to read out links
- Use the up and down arrow keys to read out items in between links
- To turn off - Right click icon in toolbar at bottom

For more keyboard shortcuts
http://webaim.org/resources/shortcuts/nvda

### VM

Download Windows 7 with IE9 (or required Windows and IE version) from:
http://modern.ie/en-us/virtualization-tools#downloads



## Tools and useful things

## Basic screen reader commands

https://www.paciellogroup.com/blog/2015/01/basic-screen-reader-commands-for-accessibility-testing/?platform=hootsuite

## Not sure how things should read out

http://maxdesign.com.au/jobs/sample-accessibility/

### Aviewer

Aviewer is a Windows tool that you can use to diagnose bugs, to see if they are a result of the screen reader or the web page.
http://www.paciellogroup.com/resources/aviewer

## Tables

### VoiceOver practice tables

http://webaim.org/articles/voiceover/tables

### Table accessibility

https://vimeo.com/139062429
