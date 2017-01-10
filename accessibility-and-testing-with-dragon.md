---
layout: page
title: Accessibility and Testing with Dragon Naturallyspeaking
---

Dragon NaturallySpeaking is a form of **speech-recognition** software, and is an invaluable tool for people who find typing difficult or painful. 

By taking away the mechanical aspects of typing, Dragon provides a more efficient way to control a computer that is less physically and cognitively taxing for those with impairments that may make typing painful or impossible. Individuals such as those with arthritis, carpal tunnel, RSI, and/or learning disabilities, face unique challenges when it comes to using a computer. The keyboard and mouse become barriers to productivity, not to mention a cause of pain and frustration.

Dragon should be tested with **Internet Explorer 11**. Test using an actual device if possible.

**Not sure how to use Dragon**? Complete the 'Interactive Tutorial', open Dragon and select 'Interactive Tutorial' under the 'Help' menu in the 'DragonBar'.

## What should I test?

0. Test the feature by navigating to it with speech
1. Test the feature by activating all the links/buttons/interactive elements as you move through the feature

## Testing steps

The accessibility acceptance criteria can be used for additional manual testing steps on device, this is written by the [Business Analyst](accessibility-news-and-business-analysts) and part of their checklist.

0. Connect headphones to PC.
1. Wear the headphones and position the microphone one inch away from your mouth.
1. Open Dragon.
2. For Dragon to hear you, it's **microphone must be on**. In the 'DragonBar', click the microphone icon to switch between on (green) or off (red).
3. Say: '**Open Internet Explorer**'.
4. Say: '**Go to address bar**'.
5. **Say the testing url**: 'www dot bbc dot co dot uk slash news'.
6. Say: '**Press enter**'.
7. **Navigate to the feature** by saying commands such as 'page down', 'line down', 'go to bottom' etc. Note, if these **commands are not working**, you do not have the browser window focussed, click in the browser window with the mouse then try again.
8. **Navigate through the feature** with the following methods:

- Tab through the feature by saying, '**tab**'. You can say commands such as 'tab 4 times' etc. to move quickly to a link/button. You should know where you are at all times. Can you see the focus styling?
- Activate each of the links in turn, by saying: '**click**' followed by the text of the link. To activate a specific link without already being focused on it, such as a story headline, say: 'Click PM pledges to improve mental health care'. If there is more than one link with a specific name such as 'UK', say 'click UK', you will then see numbers on each of the links with the text 'UK', say 'Choose 2' to choose the 2nd link with the text 'UK'. After activating a link, say '**click back**' to go back to the testing url. Note, if Dragon becomes **unresponsive**, try restarting IE and/or Dragon.
- If there are any **other interactive elements**, such a button, input field, checkbox or radio button etc. with speech test you can interact with them.

## General usage

0. By default the 'DragonBar' is minimised, hover over this to expand it.
1. In the 'DragonBar', click the microphone icon to switch between on or off. If the microphone icon is red then it is turned off, if the microphone icon is green then the microphone is turned on. Note you can only control the microphone by voice when turning it off e.g. say: 'Microphone off'.
2. When you 1st start Dragon you will see the 'Learning Centre' window, here you can see commands and tips.
3. Useful commands [cheat sheet](http://www.nuance.co.uk/ucmprod/groups/corporate/@web-enus/documents/collateral/dns13commandcheatsheet.pdf) 

### Dictation

0. Keep a consistent distance from the microphone.
1. Click where you want your dictation to go.
2. Think of your whole phrase before starting to say it.
3. Speak clearly but naturally, at a consistent volume and speed.
4. Speak punctuation and commands such as 'period' and 'new line'.
5. Text such as the word 'hello' can be edited by commands such as 'Bold hello', 'Italicize hello', 'delete hello'.
6. To correct spelling mistakes say 'correct' followed by the words to correct e.g. 'correct hello'. You will then be presented with a choice of corrections. Say 'Choose' followed by the number of the correction you would like to make.

## Test using other supported assistive technology

- [JAWS](accessibility-and-testing-with-jaws)
- [NVDA](accessibility-and-testing-with-nvda)
- [Read&Write](accessibility-and-testing-with-read-and-write)
- [Talkback](accessibility-and-testing-with-talkback)
- [VoiceOver OS](accessibility-and-testing-with-voiceover-os)
- [VoiceOver iOS](accessibility-and-testing-with-voiceover-ios)
- [ZoomText Magnifier/Reader](accessibility-and-testing-with-zoomtext)

## Other pages

- [Accessibility and Supported Assistive Technology](accessibility-and-supported-assistive-technology)