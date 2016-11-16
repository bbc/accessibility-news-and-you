---
layout: page
title: Accessibility, News and Testers
---
Accessibility testing should be done as part of the <strong>Definition of Done</strong>.

## Checklist - Automated
<ol>
<li>Check code for errors against <strong>BBC Accessibility Standards</strong>, either by using <a href="https://github.com/bbc/bbc-a11y">bbc-a11y</a> in the terminal or by using the bbc-a11y Pa11y Dashboard (Dashboard to be released early 2017).</li>

<li>Automated testing with SHIVE (HIVE for Screen Readers) - Have <strong>cucumber tests</strong> been written against the accessibility acceptance criteria? Do they pass? Note, SHIVE is not yet in production, however the tests should still be written so we are ready to go when it is.</li>

<li>Have <strong>End to End Tests</strong> been written to cover accessibility? Do they pass? A tool such as <a href="https://www.deque.com/products/axe/">Axe</a>, can be integrated, for example if using React, via <a href="https://github.com/dylanb/react-axe">React Axe</a> or the <a href="https://github.com/bbc/bbc-a11y">bbc-a11y</a> CLI could be used.</li>
</ol>

## Checklist - Manual
<ol>
<li><strong>Design</strong> - Are elements styled correctly? e.g. Do links use the standard link colour and have the standard associated hover and focus styles?</li>

<li>Do all elements meet <a href="http://www.bbc.co.uk/guidelines/futuremedia/accessibility/mobile/design/colour-contrast"><strong>colour contrast</strong></a> levels? Use a tool such as <a href="http://webaim.org/resources/contrastchecker/">contrast checker</a> to check. All colours should meet a level of 4.5:1 or higher.</li>

<li><strong>Colour blindness</strong> - Use the <a href="http://chromelens.xyz/">ChromeLens</a> dev tool extension to view the code with different vision issues.</li>

<li>Does the design use <strong>icons</strong>? Meaning should not just be conveyed with icons/images, do the icons have off-screen (visually hidden) text so users of assistive technology don't miss out? Check by inspecting the element in the web browser or with a screen reader.</li>

<li><strong>Manually check the heading order</strong>. Do the headings and the heading order actually make sense? If working on a <strong>foreign language site</strong>, use Google Translate to check what the headers actually say. You can use a tool such as the <a href="https://chrome.google.com/webstore/detail/web-developer/bfbameneiokkgbdmiekhjnmfkcnldhhm">Web Developer</a> addon for Chrome or Firefox. (Under ‘Information’ select ‘View Document Outline’ - This will show you the heading structure for the selected page.)</li>

<li><strong>Check the accessibility of the rendered DOM</strong>. Use a tool such as the <a href="https://www.deque.com/products/axe/#aXeExtensions">Axe browser extension</a>.</li>

<li><strong>Keyboard navigation</strong>
<ol>
<li> Check the <strong>tab order is correct</strong> when using the keyboard and the tab key. Can you see where you are on the page at all times e.g. Is there focus styling? This should be the same as the hover styles.
</li>
<li>Is the <strong>keyboard focus</strong> always in the correct place? e.g. After selecting a 'More' button with the return key you should be taken to the new content displayed with the next press of the tab key.</li>
<li>
When using '<strong>Trace tab path</strong>', the path should go from left to right as you work your way down the page (there will be some exceptions to this order, such as when the 'Breaking news' banner is on the page). Use the <a href="http://chromelens.xyz/">ChromeLens</a> dev tool extension to trace the tab path.</li>
</ol>
<li><strong>Has the feature been considered without javascript</strong>? It should degrade gracefully. Use a tool such as the <a href="https://chrome.google.com/webstore/detail/web-developer/bfbameneiokkgbdmiekhjnmfkcnldhhm">Web Developer</a> addon for Chrome or Firefox to easily turn Javascript off.</li>
</ol>

## Checklist - Assistive Technology

Test with <a href="accessibility-and-supported-assistive-technology">Supported Assistive Technology</a>, using an actual device if possible.

<ol>
<li>Is the feature useable?</li>
<li>Does the feature make sense?</li>
</ol>

### Checklists for other roles in the team

- <a href="accessibility-news-and-product-owners">Product Owner</a>
- <a href="accessibility-news-and-designers">Designer</a>
- <a href="accessibility-news-and-business-analysts">Business Analyst</a>
- <a href="accessibility-news-and-developers">Developer</a>
