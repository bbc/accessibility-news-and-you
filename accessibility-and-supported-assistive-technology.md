---
layout: page
title: Accessibility and Supported Assistive Technology
---
Based on the results from the [2016 GOV.UK Assistive Technology Survey](https://accessibility.blog.gov.uk/2016/11/01/results-of-the-2016-gov-uk-assistive-technology-survey/).

Test on an actual device if possible. Is the feature useable, does it make sense?

See the [AT Set Up Guide](Testing-with-a-Screen-reader) for usage instructions.

# Priority 1 (P1)

To meet the **Definition of Done** the following should be used for testing.

0. **ZoomText Magnifier/Reader** Latest Version<br>
With Internet Explorer 11 on Windows (XP/Vista/7/8/10)<br>
(Screen Magnifier with Screen Reader capabilities)

0. **Dragon Naturallyspeaking** Version 13<br>
With Internet Explorer 11 on Windows (XP/Vista/7/8/10)<br>
(Speech Recognition)

0. **JAWS** Version 17<br>
With Internet Explorer 11 on Windows (XP/Vista/7/8/10)<br>
(Screen Reader)

0. **Read and Write** Latest Version<br>
With Internet Explorer 11 on Windows (XP/Vista/7/8/10)<br>
(Reading Solution)

0. **VoiceOver** Latest Version<br>
With Safari (Latest Version) on iOS (Latest Version)<br>
(Screen Reader)

# Priority 2 (P2)

If time allows the following should also be used for testing.

0. **NVDA** (Latest Version)<br>
With Firefox (Latest Version) on Windows (XP/Vista/7/8/10)<br>
(Screen Reader)

# Priority 3 (P3)

If time further allows the following should also be used for testing.

0. **VoiceOver** (Latest Version)<br>
With Safari (Latest Version) on Mac OS (Latest Version)<br>
(Screen Reader)

0. **Talkback** (Latest Version)</br>
With Chrome (Latest Version) on Android (Latest Version)<br>
(Screen Reader)

# Why do we base our testing on the GOV.UK survey

The GOV.UK Assistive Technology Survey is the only survey of it's type carried out in the UK and therefore we base our testing matrix on this and combine this with other knowledge about our audience, such as we know that we have a large mobile audience and therefore put VoiceOver on iOS into the P1 category.

## Translating the statistics

### 30% of respondents used a screen magnifier

38% of the magnifiers have screen reader capabilities.

0. **ZoomText** 54.3% (**16.3% of total**)
0. Supernova 10.9% (3.3% of total)
0. Magic 3.9% (1.2% of total)
0. Other 17.1% (5.1% of total)
0. Don't know 14% (4.2% of total)

### 29% of respondents used a screen reader

0. **Jaws** 38.5% (**11.2% of total**)
0. **VoiceOver** 21.2 (6.1% of total)<br>
  0. (72% of this on **iOS**, **4.4% of total**)
  0. (28% of this on macOS, 1.7% of total)
0. **NVDA** 12% (**3.5% of total**)
0. Supernova 3.8% (1.1% of total)
0. WindowEyes 2.9% (0.8% of total)
0. Guide 2.4% (0.7% of total)
0. Talkback 1.9% (0.6% of total)
0. Narrator 1% (0.3% of total)
0. ChromeVox 1% (0.3% of total)
0. Orca 0.5% (0.1% of total)
0. Other 7.7% (2.2% of total)
0. Don't know 7.2% (2.1% of total)

### 18% of respondents used speech recognition

0. **Dragon Naturallyspeaking** 84.3% - Versions 11, 12 & 13 (**15.2% of total**)
0. Other 7.4% (1.3% of total)
0. Don't know 5.5% (0.9% of total)

### 15% of respondents used a reading solution

Reading solutions are aimed at users who have dyslexia.

0. **Read and Write** 68.4% (**10.3% of total**)
0. ClaraRead 6.1% (0.9% of total)

The survey says that a number of Read and Write users also have Dragon Naturallyspeaking running in tandem.

### Highest total usage (from all categories)

0. ZoomText 16.3%
0. Dragon 15.2%
0. Jaws 11.2%
0. Read and Write 10.3%
0. VoiceOver on iOS 4.4%
0. NVDA 3.5%
