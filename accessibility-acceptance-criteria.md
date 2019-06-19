---
layout: page
title: A guide to writing accessibility acceptance criteria
---
Accessibility acceptance criteria is one of the practices that helps us meet the **[BBC Accessibility Guidelines](https://www.bbc.co.uk/accessibility/forproducts/guides/mobile/)**.

Here accessibility acceptance criteria defines conditions for elements:

- That play a key part in a component being accessible
- That are at high risk of introducing an accessibility issue

Write this where relevant, for **new components and iterations before the development phase**. Note, this guide uses the **[GDS approach](https://insidegovuk.blog.gov.uk/2018/01/24/improving-accessibility-with-accessibility-acceptance-criteria/)** as a basis, there are other ways that you could approach this. We will use the following steps:

0. **[Accessibility design review confirmation](#1-accessibility-design-review-confirmation)**
1. **[Gather documentation](#2-gather-documentation)**
2. **[List key and high risk elements](#3-list-key-and-high-risk-elements)**
3. **[Write the scenarios](#4-write-the-scenarios)**
4. **[Make everyone aware](#5-make-everyone-aware)**

## 1) Accessibility design review confirmation
Confirm if the component you are writing criteria for has had a **[review for accessibility](accessibility-design-review)**. If this hasn’t taken place, ask UX to carry out a review before proceeding to the next step.

## 2) Gather documentation
Gather the following documentation. This will form a basis for writing the accessibility acceptance criteria:

- Documented visual user experience
- Documented screen reader UX

Ask UX for this documentation if it's missing, before proceeding to the next step.

## 3) List key and high risk elements
Hold a **[Three Amigos](https://en.wikipedia.org/wiki/Behavior-driven_development#The_Three_Amigos)** session including a **designer** and **accessibility champion**. Here you should use the gathered documentation to **make a list** of elements:

- **[That play a key part in a component being accessible](#examples-of-elements-that-play-a-key-part-in-a-component-being-accessible)**
- **[That are at high risk of introducing an accessibility issue](#examples-of-elements-that-are-at-high-risk-of-introducing-an-accessibility-issue)**

Alongside the gathered documentation, **use guidelines to help you** identify elements. Note, you do not need to identify and list everything that would make the component accessible. Your aim isn’t to reproduce guidelines, such as:

- **[BBC Accessibility Guidelines](https://www.bbc.co.uk/accessibility/forproducts/guides/mobile/)**
- **[WCAG](https://www.w3.org/TR/WCAG21/)**
- **[WAI-ARIA Authoring Practices](https://www.w3.org/TR/wai-aria-practices-1.1/)**
- **[ARIA states and properties](https://www.w3.org/TR/wai-aria-1.1/#state_prop_def)**
- **[ARIA landmarks examples](https://www.w3.org/TR/2017/NOTE-wai-aria-practices-1.1-20171214/examples/landmarks/index.html)**

Need an example? See **[example list of key and high risk elements for an ordered list component](#example-list-of-key-and-high-risk-elements-for-an-ordered-list-component)**.

## 4) Write the scenarios
Write scenarios for all listed elements. Use the **Given, When, Then** approach that is used in **[Behaviour Driven Development](https://en.wikipedia.org/wiki/Behavior-driven_development)**. This format will help everyone understand each of the listed elements.

Things to remember:

- **Use guidelines and documentation** - Extract relevant rules or information. If appropriate link back to guidelines for reference.

- **Don’t specify a solution** - Engineers can consider the best solution to achieve the defined criteria. If the component styling or assistive technology changes, the criteria should still apply.

- **Be consistent** - If you have defined similar criteria before, replicate the format.

Need an example? See **[example scenarios for an ordered list component](#example-scenarios-for-an-ordered-list-component)**.

## 5) Make everyone aware
The criteria should be visible to all the team, including engineers and non-technical team members.

## Examples

### Examples of elements that play a key part in a component being accessible

- **Announced text** - Besides the text that you can see, is there any extra text that needs announcing to screen reader users? To avoid missing meaning or context? For example text alternatives for icons.

- **Content order** - Is the content order in the screen reader UX different to the visual user experience? For example, you might position a close button in the top righthand corner of a component. We can improve the screen reader UX by announcing the button at the end of the component.

- **Extra meaning** - Is the screen reader UX improved by reinforcing or providing extra semantics? For example, accordions that expand or collapse content have an arrow icon to convey this. This meaning should also convey to screen reader users. Such as via the aria-expanded attribute.

- **HTML markup** - A sighted user can identify elements and their meaning by looking at them. For example, they can identify a heading because the font size is usually larger than that of other text. For screen reader users you need to convey that meaning by using semantic HTML markup. In this case by using a HTML heading element.

- **Landmarks** - Does the screen reader UX include any ARIA landmarks? For the component itself and/or should the component sit within a specific landmark? Such as a navigation element within a banner landmark.

- **Tab order** - Does keyboard focus need to move to a particular element after an in-page interaction? For example, when activating a ‘Show more updates’ button. Focus will need to move to the new content if displayed above the button in the content order.

- **Visually hidden content** - Are there any elements in the screen reader UX that you don’t have in the visual user experience? Such as heading that isn't needed visual design.

**[Back to 'list key and high risk elements'](#3-list-key-and-high-risk-elements)**

### Examples of elements that are at high risk of introducing an accessibility issue

- **Colour contrast** - A component’s use of colour can increase the risk of introducing an accessibility issue. Imagine dark grey text on a light grey background, this may meet colour contrast levels. A slight change of shade to one of the greys, is at high risk of reducing colour contrast to an unacceptable level.

- **Headings** - Correct use of heading levels within components is important to screen reader users. The change of a heading levels is at high risk of breaking the page heading structure.

- **Hidden content** - Is there any hidden content? Such as an unexpanded menu. If the menu isn't hidden correctly, it's at at high risk of introducing an accessibility issue. The menu items could be available to screen reader users when they shouldn't be.

**[Back to 'list key and high risk elements'](#3-list-key-and-high-risk-elements)**

### Example list of key and high risk elements for an ordered list component

If the component was an ordered list, you could list the key and high risk elements as:

0. List semantics for screen reader users
1. List item numbers must be announced to screen reader users
2. List item numbers must meet the colour contrast ratio of 4.1:5
3. Read from left to right when in 2 columns or more

**[Back to 'list key and high risk elements'](#3-list-key-and-high-risk-elements)**

### Example scenarios for an ordered list component
In our example, using the list of key and high risk elements for an ordered list, the scenarios could be:

- Given I use a screen reader
- When navigating to an ordered list
- Then it should be announced as a list

- Given I use a screen reader
- When navigating to a list item in an ordered list
- Then the text should be announced 
- And it should be prefixed by the announcement of the list number

- Given I am viewing an ordered list
- When the list item number is a different colour to the text 
- Then the number must meet the colour contrast ratio of 4.1:5

- Given I am viewing an ordered list
- When the list items are displayed in 2 columns or more
- Then each column must read from left to right

**[Back to 'write the scenarios'](#4-write-the-scenarios)**
