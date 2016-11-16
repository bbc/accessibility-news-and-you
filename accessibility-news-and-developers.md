---
layout: page
title: Accessibility, News and Developers
---
Accessibility should be considered from the start of development and throughout the process.

## Checklist - Before development starts
<ol>
<li>Question/Check the <strong>design</strong> you are working from. Are elements styled correctly? e.g. Do links use the standard link colour and have the standard associated hover and focus styles? Do all elements meet <a href="http://www.bbc.co.uk/guidelines/futuremedia/accessibility/mobile/design/colour-contrast">colour contrast</a> levels? Use a tool such as <a href="http://webaim.org/resources/contrastchecker/">contrast checker</a> to check. All colours should meet a level of 4.5:1 or higher.</li>

<li>Does the design use <strong>icons</strong>? Meaning should not just be conveyed with icons/images, do the icons need some off-screen (visually hidden) text so users of assistive technology don't miss out? If so, what would this text be?</li>

<li>Consider the mark up. <strong>Semantic HTML</strong> should be used, this way you get accessibility from the start.</li>
</ol>

## Checklist - Throughout development
<ol>

<li>Use a <strong>linting tool with accessibility rules</strong> added to catch errors as you develop, for example if using React, <a href="https://github.com/bbc/morph-with-grandstand/blob/master/README.md#jsx-a11y">eslint plugin jsx-ally</a> should be installed in your module if it isn't already.</li>

<li><strong>Check the accessibility of the rendered DOM</strong>. Use a tool such as the <a href="https://www.deque.com/products/axe/#aXeExtensions">Axe browser extension</a>.</li>

<li><strong>Turn CSS off in the browser</strong>. Does the page make sense, is it easily understandable? Is the correct mark up used for the correct elements? e.g. If there is a button, is it marked up as a button? If there is a list, is it marked up as a list? Do components have headers? Use a tool such as the <a href="https://chrome.google.com/webstore/detail/web-developer/bfbameneiokkgbdmiekhjnmfkcnldhhm">Web Developer</a> addon for Chrome or Firefox to easily turn CSS off.</li>

<li><strong>Have you considered the page without javascript</strong>? It should degrade gracefully. Use a tool such as the <a href="https://chrome.google.com/webstore/detail/web-developer/bfbameneiokkgbdmiekhjnmfkcnldhhm">Web Developer</a> addon for Chrome or Firefox to easily turn Javascript off.</li>

<li><strong>Keyboard navigation</strong>
<ol>
<li> Check the <strong>tab order is correct</strong> when using the keyboard and the tab key. Can you see where you are on the page at all times e.g. Have you set focus styling? This should be the same as the hover styles.
</li>
<li>Is the <strong>keyboard focus</strong> always in the correct place? e.g. After selecting a 'More' button with the return key you should be taken to the new content displayed with the next press of the tab key.</li>
<li>
When using '<strong>Trace tab path</strong>', the path should go from left to right as you work your way down the page (there will be some exceptions to this order, such as when the 'Breaking news' banner is on the page). Use the <a href="http://chromelens.xyz/">ChromeLens</a> dev tool extension to trace the tab path.</li>
</ol>
<li>Do you need to use any <a href="https://www.w3.org/WAI/intro/aria.php"><strong>ARIA</strong></a>? For example, ARIA can be used simply to add landmarks/regions to a page or more advanced usage can help with dynamic content and advanced user interface controls such as tabs. For examples see <a href="http://w3c.github.io/aria-practices/">ARIA Authoring Practices</a>. Note ARIA should be used sparingly.</li>
<li>Use <a href="Testing-with-a-Screen-reader"><strong>VoiceOver</strong></a> (screen reader) on iOS during development. It's a lot more effort to fix bugs after you are code complete.</li>
</ol>

## Checklist - Before code merge
<ol>
<li><strong>Manually check the heading order</strong>. Do the headings and the heading order actually make sense? If working on a <strong>foreign language site</strong>, use Google Translate to check what the headers actually say. You can use a tool such as the <a href="https://chrome.google.com/webstore/detail/web-developer/bfbameneiokkgbdmiekhjnmfkcnldhhm">Web Developer</a> addon for Chrome or Firefox. (Under ‘Information’ select ‘View Document Outline’ - This will show you the heading structure for the selected page.)</li>

<li><strong>Colour blindness</strong> - Use the <a href="http://chromelens.xyz/">ChromeLens</a> dev tool extension to view the code with different vision issues. Let UX know if there are some concerns.</li>

<li>Specifically check your code for errors against <strong>BBC Accessibility Standards</strong>, either by using <a href="https://github.com/bbc/bbc-a11y">bbc-a11y</a> in the terminal or by using the bbc-a11y Pa11y Dashboard (Dashboard to be released early 2017).</li>

<li>Test with <a href="Accessibility-and-Supported-Assistive-Technology">Assistive Technology</a> that we support</li>

<li>Automated testing with SHIVE (HIVE for Screen Readers) - Have <strong>cucumber tests</strong> been written against the accessibility acceptance criteria? Note, SHIVE is not yet in production, however the tests should still be written so we are ready to go when it is.</li>

<li>Have <strong>End to End Tests</strong> been written to cover accessibility? A tool such as <a href="https://www.deque.com/products/axe/">Axe</a>, can be integrated, for example if using React, via <a href="https://github.com/dylanb/react-axe">React Axe</a> or the <a href="https://github.com/bbc/bbc-a11y">bbc-a11y</a> CLI could be used.</li>
</ol>

### Checklists for other roles in the team
- <a href="accessibility-news-and-product-owners">Product Owner</a>
- <a href="accessibility-news-and-designers">Designer</a>
- <a href="accessibility-news-and-business-analysts">Business Analyst</a>
- <a href="accessibility-news-and-developers">Developer</a>
- <a href="accessibility-news-and-testers">Tester</a>
