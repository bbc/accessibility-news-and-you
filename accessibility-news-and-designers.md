---
layout: page
title: Accessibility, News and Designers
---
Design with accessibility in mind from the start.

Some simple quick checks are outlined here, please refer to the <a href="http://www.bbc.co.uk/guidelines/futuremedia/accessibility/">BBC Accessibility Standards and Guidelines</a> for in depth information.

Do you have an understanding of what <a href="Accessibility-and-Supported-Assistive-Technology">Assistive Technology we support</a>, such as screen readers? And how to use this?

For an introduction on accessible thinking see the <a href="http://www.bbc.co.uk/gel/guidelines/how-to-design-for-accessibility">How to Design for Accessibility</a> guide. It is also recommended to attend the Accessible UX course and complete the <a href="http://www.bbc.co.uk/academy/beta/course/COU-12887">Accessibility for Web Developers</a> online course. The <a href="http://www.bbc.co.uk/academy/beta/course/COU-50344015">Introduction to Screen Readers</a> course would also be very useful.

## Design checks

For designs created using Sketch or Photoshop etc.

### Checklist - Throughout the design process

<ol>
<li>Are elements styled correctly? e.g. Do links use the standard link colour and standard associated hover and focus styles? A consistent experience is good for accessibility.</li>

<li>Do all elements meet <a href="http://www.bbc.co.uk/guidelines/futuremedia/accessibility/mobile/design/colour-contrast">colour contrast</a> levels? Use a tool such as <a href="http://webaim.org/resources/contrastchecker/">contrast checker</a> to check. All colours should meet a level of 4.5:1 or higher.</li>

<li>Does your design work for colour blindness? Drop a jpg/gif of your design into Chrome and use the <a href="http://chromelens.xyz/">ChromeLens</a> dev tool extension to view your design with different vision issues.</li>

<li>Does your design pass the <a href="https://accessibility.blog.gov.uk/2016/09/02/dos-and-donts-on-designing-for-accessibility">Dos and Don'ts of Designing for Accessibility</a>?</li>

<li>Have you considered the page without javascript? It should degrade gracefully.</li>
</ol>

### Checklist - Before design sign off

<ol>
<li>Accessibility Champion Review - Get your designs peer reviewed, from a champion in the product/feature team, before sign off and/or development starts.</li>

<li>Does your design use icons? Meaning should not just be conveyed with images, do the icons need some off-screen (visually hidden) text so users of assistive technology don't miss out? If so, what would this text be?</li>

<li>Think about the HTML, how will this be marked up? Have you thought about the <a href="http://www.bbc.co.uk/guidelines/futuremedia/accessibility/html/headings.shtml">heading</a> structure? Do you know what heading level your headings are and how this will fit into the rest of the page? Do you need to use any <a href="https://www.w3.org/WAI/intro/aria.php">ARIA</a>? For example, ARIA can be used simply to add landmarks/regions to a page or more advanced usage can help with dynamic content and advanced user interface controls such as tabs. For examples see <a href="http://w3c.github.io/aria-practices/">ARIA Authoring Practices</a>. Note ARIA should be used sparingly.</li>

<li>Have you thought about keyboard navigation, is the tab order logical? e.g. When using the keyboard and the tab key, the tab order should go from left to right as you work your way down the page (there will be some exceptions to this order, such as when the 'Breaking news' banner is on the page).</li>
</ol>

### Checklist - When on test or live

<ol>
<li>Test your design with assistive technology, such as a screen reader, <a href="Testing-with-a-Screen-reader">VoiceOver</a> on iOS is recommended, does it make sense?</li>
<li>You can use the bbc-a11y Pa11y Dashboard to check for code errors against the BBC Accessibility Standards. Note passing the standards does not mean a product is useable. This dashboard to be released early 2017.</li>
</ol>

### Checklists for other roles in the team
- <a href="Accessibility,-News-and-Product-Owners">Product Owner</a>
- <a href="Accessibility,-News-and-Business-Analysts">Business Analyst</a>
- <a href="Accessibility,-News-and-Developers">Developer</a>
- <a href="Accessibility,-News-and-Testers">Tester</a>
