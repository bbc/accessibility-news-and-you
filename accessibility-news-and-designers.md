---
layout: page
title: Accessibility, News and Designers
---
Design with accessibility in mind from the start.

Some simple quick checks are outlined here, please refer to the [BBC Accessibility Standards and Guidelines](http://www.bbc.co.uk/guidelines/futuremedia/accessibility/) for in depth information.

Do you have an understanding of what [Assistive Technology we support](accessibility-and-supported-assistive-technology), such as screen readers? And how to use this?

For an introduction on accessible thinking see the [How to Design for Accessibility](http://www.bbc.co.uk/gel/guidelines/how-to-design-for-accessibility) guide. It is also recommended to attend the Accessible UX course and complete the [Accessibility for Web Developers](http://www.bbc.co.uk/academy/beta/course/COU-12887) online course. The [Introduction to Screen Readers](http://www.bbc.co.uk/academy/beta/course/COU-50344015) course would also be very useful.

## Design checks

For designs created using Sketch or Photoshop etc.

### Checklist - Throughout the design process

0. Are elements styled correctly? e.g. Do links use the standard link colour and standard associated hover and focus styles? A consistent experience is good for accessibility.

0. Do all elements meet [colour contrast](http://www.bbc.co.uk/guidelines/futuremedia/accessibility/mobile/design/colour-contrast) levels? Use a tool such as [contrast checker](http://webaim.org/resources/contrastchecker/) to check. All colours should meet a level of 4.5:1 or higher.

0. Does your design work for colour blindness? Drop a jpg/gif of your design into Chrome and use the [ChromeLens](http://chromelens.xyz/) dev tool extension to view your design with different vision issues.

0. Does your design pass the [Dos and Don'ts of Designing for Accessibility](https://accessibility.blog.gov.uk/2016/09/02/dos-and-donts-on-designing-for-accessibility)?

0. Have you considered the page without javascript? It should degrade gracefully.

### Checklist - Before design sign off

0. Accessibility Champion Review - Get your designs peer reviewed, from a champion in the product/feature team, before sign off and/or development starts.

0. Does your design use icons? Meaning should not just be conveyed with images, do the icons need some off-screen (visually hidden) text so users of assistive technology don't miss out? If so, what would this text be?

0. Think about the HTML, how will this be marked up? Have you thought about the [heading](http://www.bbc.co.uk/guidelines/futuremedia/accessibility/html/headings.shtml) structure? Do you know what heading level your headings are and how this will fit into the rest of the page? Do you need to use any [ARIA](https://www.w3.org/WAI/intro/aria.php)? For example, ARIA can be used simply to add landmarks/regions to a page or more advanced usage can help with dynamic content and advanced user interface controls such as tabs. For examples see [ARIA Authoring Practices](http://w3c.github.io/aria-practices/). Note ARIA should be used sparingly.

0. Have you thought about keyboard navigation, is the tab order logical? e.g. When using the keyboard and the tab key, the tab order should go from left to right as you work your way down the page (there will be some exceptions to this order, such as when the 'Breaking news' banner is on the page).

### Checklist - When on test or live

0. Test your design with assistive technology, such as a screen reader, [VoiceOver](testing-with-a-screen-reader) on iOS is recommended, does it make sense?
0. You can use the bbc-a11y Pa11y Dashboard to check for code errors against the BBC Accessibility Standards. Note passing the standards does not mean a product is useable. This dashboard to be released early 2017.

### Checklists for other roles in the team

- [Product Owner](accessibility-news-and-product-owners)
- [Business Analyst](accessibility-news-and-business-analysts)
- [Developer](accessibility-news-and-developers)
- [Tester](accessibility-news-and-testers)
