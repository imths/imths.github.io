---
layout: essay
type: essay
title: "Keeping Code Clean"
date: 2024-02-08
published: true
labels:
  - Computer Science
  - Software Engineering
---

<img height="200px" class="img-thumbnail" src="../img/code-standards/Coding-Standards.jpg">

Coding standards are certain rules and habits that programmers are generally expected to follow when creating/writing code and working on projects with collaborators or partners. By implementing coding standards in a team based environment, all code should be formatted in a way that it is easier to read and understand for any existing member or future team members who join later on and will likely not have any prior knowledge of the project. This ensures that everyone is on the same page with one another, which can then result in easier collaboration and any questions are able to be answered by more than just a single person.

## Learning with and without Coding Standards

<img height="200px" class="img-thumbnail" src="../img/code-standards/coding-confusion.png">

When learning a new programming language, it is important that the examples given to you are easily digestible and understandable, to ensure that you are able to then take that knowledge and apply it to any other scenario you deem fit. The same can be said for more hands-on or on the site learning, where you are thrown into the working environment, and forced to learn what you can about the languages being used in a project and how they are actually being used. In these situations, without clean and comprehensible code, learning becomes much tougher than it should be, and would likely take more time and effort put forward to actually learning the language, making progress almost nonexistent. Being able to practice with coding standards also builds good habits in programming and working with any language, and making sure to keep up with the standards and conventions for the code will ensure that you are thinking about what you are doing in your code, and how to format everything to the best of your abilities.

## First? Impressions of ESLint in IntelliJ

<img height="200px" class="img-thumbnail" src="../img/code-standards/linters.png">

As of late last year, 2023, I began working as a Web App Developer with the UH Manoa ITS IAM team, which is where I first began my experience with Git and IntelliJ IDEA, working with languages such as HTML, (S)CSS, Java, JavaScript, TypeScript, etc. and building up my experience and confidence in working with front and back end programming. Having worked with IntelliJ a bit before being fully introduced to ESLint and linters in general, I was aware of coding standards and that IntelliJ provided plugins and settings to help upkeep these standards and warn users of "messy" code, but it was never fully emphasized for us to use ESLint specifically. I was already used to attempting to make my code "neat" or "readable", and the idea of linters are not new to me, but there will always be some small details that I miss, or do not realize might cause possible problems in the future, that ESLint will catch and return for me to fix.

## Code Cleanup Crew

<img height="200px" class="img-thumbnail" src="../img/code-standards/eslint-problems.png">

When it comes to fixing the problems returned to me by ESLint, as long as I understand the idea behind what is wrong, I usually do not have any major problems in getting rid of the red 'X' and getting the green check to show up. If I do not have much of an understanding of what is wrong, I will usually just take IntelliJ's suggestions on how to fix the "problem" by clicking on the lightbulb in the editor. One tool/feature that I find very useful when working in IntelliJ, is the "Problems" tab in the editor, that returns and displays any code warnings with a brief description of what is "wrong", as well as the line that the problem can be found on. It is possible to jump to these warning locations through this screen as well, by just double clicking on the warning itself in the tab, which is useful for bigger files and projects.
