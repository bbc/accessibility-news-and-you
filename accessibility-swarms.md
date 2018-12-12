---
layout: page
title: Accessibility Swarms
---
Accessibility Swarms are a practice that we carry out in BBC News. We do this because **accessibility is a team responsibility**.

Swarms take place on **all new front-end code**, this means any changes to HTML, CSS or JavaScript code.

## When should you carry out a swarm?
- Before a ticket moves from Development to Test
- When HTML, CSS & JS is code complete (including code review)
- Some developer testing with some assistive technology should already have taken place

## Who takes part?
### If it’s a new component or feature
Carry out a **team swarm**, with 4 to 6 people.

- You don’t need to have worked on the ticket
- All disciplines can join in. The **[testing steps](accessibility-and-testing-with-assistive-technology)** enable anyone, in any role, to use any of the assistive technology for the first time.
- Ideally you want a mix of roles such as Business Analyst, Designer and Developer
- If you don't have a large team, why not invite people from another team to take part. And you can return the favour for them sometime.

### If it’s a small change
Carry out a **developer swarm**.

- You don’t need 4 to 6 people
- 2 developers can work through the **[checklist](accessibility-news-and-testers)** alone
- You only need to check what’s relevant. For example, if you have only changed a colour, then you only need to check what’s relevant to this. Such as, colour contrast and colour blindness.

## Planning for swarms
The level of Accessibility Swarm (team or developer swarm) should be defined up front. So that planning sessions can include Accessibility Swarm effort. 

## How to carry out a swarm
- Get the equipment you need:
    - Mac laptop
    - PC laptop with **[supported assistive technology](accessibility-and-supported-assistive-technology)** installed
    - Headphones with microphone to use with Dragon NaturallySpeaking e.g. Jabra headset
    - iPhone or iPad
    - Android phone with Talkback 
- Grab a space
- Get into pairs, a technical role with a non-technical role. Such as Developer and Designer working together.
- Brief the swarmers – Is there something that you need to look out for that might not be obvious? Such as, off screen visually hidden text etc.
- Work through the **[checklist](accessibility-news-and-testers)**
- Test with all **[supported assistive technology](accessibility-and-supported-assistive-technology)** following the **[testing steps](accessibility-and-testing-with-assistive-technology)**
- Make notes of any issues
- Prioritise bugs

After the swarm, create tickets to fix the issues you aren't going to address in your current pull request. Include information on how to replicate the issue and the priority level.

## How long will the swarm take?
- Some swarms will be shorter, some longer
- Allow 2 hours
- It will depend on the size and complexity of the component, and experience of the swarmers

## When a ticket moves to Test
- Confirm if an Accessibility Swarm has taken place and what was tested during the swarm 
- If the checklist was not completed, fill in the gaps to ensure you have complete testing coverage
- If the code hasn’t changed since the swarm, you **do not** need to repeat what was carried out in the swarm
- Test against Accessibility Acceptance Criteria
- If time, test with assistive technology  using more devices and operating system versions

## Be proactive
- Any role can start a swarm – Business Analyst, Designer, Developer etc.
- Product Owners, Project Managers & Testers should be asking if a swarm has taken place on a ticket

## Top tips
- Work at component level rather than page level
- The more swarms you do, the more familiar and faster you will get
- Always follow the **[testing steps](accessibility-and-testing-with-assistive-technology)**
- Not sure? Ask an Accessibility Champion
