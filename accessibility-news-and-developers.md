---
layout: page
title: Accessibility, News and Developers
---
Accessibility should be considered from the start of development and throughout the process.

0. Are you aware of the [BBC Accessibility Standards and Guidelines](http://www.bbc.co.uk/guidelines/futuremedia/accessibility/)? Some simple quick checks are outlined here, please refer to the guidelines for in depth information.

0. Do you have an understanding of what [Assistive Technology we support](accessibility-and-supported-assistive-technology), such as screen readers? And how to use this?

To gain an understanding of accessibility features and what to look for it is recommended to attend the Accessible UX course and complete the [Accessibility for Web Developers](http://www.bbc.co.uk/academy/beta/course/COU-12887) <small>(Internal BBC link)</small> online course. The [Introduction to Screen Readers](http://www.bbc.co.uk/academy/beta/course/COU-50344015) <small>(Internal BBC link)</small> course would also be very useful.

## Checklist - Before development starts

0. Question/Check the **design** you are working from. Are elements styled correctly? e.g. Do links use the standard link colour and have the standard associated hover and focus styles? Do all elements meet [colour contrast](http://www.bbc.co.uk/guidelines/futuremedia/accessibility/mobile/design/colour-contrast) levels? Use a tool such as [contrast checker](http://webaim.org/resources/contrastchecker/) to check. All colours should meet a level of 4.5:1 or higher.

0. Does the design use **icons**? Meaning should not just be conveyed with icons/images, do the icons need some off-screen (visually hidden) text so users of assistive technology don't miss out? If so, what would this text be?

0. Consider the mark up. **Semantic HTML** should be used, this way you get accessibility from the start.

## Checklist - Throughout development

0. Use a **linting tool with accessibility rules** added to catch errors as you develop, for example if using React, [the jsx-a11y ESLint plugin](https://www.npmjs.com/package/eslint-plugin-jsx-a11y) should be installed in your module if it isn't already.

0. **Check the accessibility of the rendered DOM**. Use a tool such as the [Axe browser extension](https://www.deque.com/products/axe/#aXeExtensions).

0. **Turn CSS off in the browser**. Does the page make sense, is it easily understandable? Is the correct mark up used for the correct elements? e.g. If there is a button, is it marked up as a button? If there is a list, is it marked up as a list? Do components have headers? Use a tool such as the [Web Developer](https://chrome.google.com/webstore/detail/web-developer/bfbameneiokkgbdmiekhjnmfkcnldhhm) add-on for Chrome or Firefox to easily turn CSS off.

0. **Have you considered the page without javascript**? It should degrade gracefully. Use a tool such as the [Web Developer](https://chrome.google.com/webstore/detail/web-developer/bfbameneiokkgbdmiekhjnmfkcnldhhm) add-on for Chrome or Firefox to easily turn Javascript off.

0. **Keyboard navigation**
    0. Check the **tab order is correct** when using the keyboard and the tab key. Can you see where you are on the page at all times e.g. Have you set focus styling? This should be the same as the hover styles.

    0. Is the **keyboard focus** always in the correct place? e.g. After selecting a 'More' button with the return key you should be taken to the new content displayed with the next press of the tab key.

    0. When using '**Trace tab path**', the path should go from left to right as you work your way down the page (there will be some exceptions to this order, such as when the 'Breaking news' banner is on the page). Use the [ChromeLens](http://chromelens.xyz/) dev tool extension to trace the tab path.

0. Do you need to use any [**ARIA**](https://www.w3.org/WAI/intro/aria.php)? For example, ARIA can be used simply to add landmarks/regions to a page or more advanced usage can help with dynamic content and advanced user interface controls such as tabs. For examples see [ARIA Authoring Practices](http://w3c.github.io/aria-practices/). Note ARIA should be used sparingly.

0. Use **VoiceOver** (Screen Reader) on iOS during development. It's a lot more effort to fix bugs after you are code complete. If using VoiceOver for the 1st time, see the [Assistive Technology Setup Guide](assistive-technology-set-up-guide).

## Checklist - Before code merge

0. **Manually check the heading order**. Do the [heading](http://www.bbc.co.uk/guidelines/futuremedia/accessibility/html/headings.shtml) and the heading order actually make sense? If working on a **foreign language site**, use Google Translate to check what the headers actually say. You can use a tool such as the [Web Developer](https://chrome.google.com/webstore/detail/web-developer/bfbameneiokkgbdmiekhjnmfkcnldhhm) add-on for Chrome or Firefox. (Under ‘Information’ select ‘View Document Outline’ - This will show you the heading structure for the selected page.)

0. **Colour blindness** - Use the [ChromeLens](http://chromelens.xyz/) dev tool extension to view the code with different vision issues. Let UX know if there are some concerns.

0. Specifically check your code for errors against **BBC Accessibility Standards**, either by using [bbc-a11y](https://github.com/bbc/bbc-a11y) in the terminal or by using the bbc-a11y Pa11y Dashboard (Dashboard to be released early 2017).

0. Test with [Assistive Technology](accessibility-and-supported-assistive-technology) that we support

0. Automated testing with SHIVE (HIVE for Screen Readers) - Have **cucumber tests** been written against the accessibility acceptance criteria? Note, SHIVE is not yet in production, however the tests should still be written so you are ready to go when it is.

0. Have **End to End Tests** been written to cover accessibility? A tool such as [Axe](https://www.deque.com/products/axe/), can be integrated, for example if using React, via [React Axe](https://github.com/dylanb/react-axe) or the [bbc-a11y](https://github.com/bbc/bbc-a11y) CLI could be used.

## Checklists for other roles in the team

- [Product Owner](accessibility-news-and-product-owners)
- [Designer](accessibility-news-and-designers)
- [Business Analyst](accessibility-news-and-business-analysts)
- [Tester](accessibility-news-and-testers)
