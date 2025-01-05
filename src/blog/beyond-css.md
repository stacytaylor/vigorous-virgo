---
title: "CSS Architecture with Beyond CSS"
description: ""
pubDate: 2024-08-19
tags: ["css", "design engineering" ]
---

## The gap in CSS courses

I’ve been dabbling in CSS for well over a decade at this point and have taken a number of different courses from different platforms. And what I’ve found is that many of them teach the same basic concepts over and over. You’ve got your basic introduction to CSS, including how to add styles to your websites and the basics of specificity and inheritance. Then you’ve got your “responsive web design” courses that focus on flexbox and grid. But after that? I’d seen enough code to know that most devs use things like utility classes and variables, but these things never seemed to get covered in the courses I found. Enter Beyond CSS.

## Moving Beyond

Kevin Powell’s new [Beyond CSS course] <https://www.beyondcss.dev/> was exactly what I was looking for. He starts by introducing Sass (and SCSS), covering concepts like nested selectors, variables, and mixins in module one. In module two he moves on to the more advanced features of SCSS, using functions to add logic to your stylesheets. But module three is where we really start cooking with fire.

## Building scalable systems

### Troubleshooting woes

Module three starts by introducing Vite to create a starter template to use throughout the rest of the course. I’ll confess I got a bit lost during this section. There’s a couple of errors in the course where Kevin uses different names for the same file at various points in the lessons and I lost half a day trying to troubleshoot why I couldn’t get my CSS to compile.

The module also suffered from the same issue I see in many courses – a new tool is introduced, and the teacher just gives you a list of commands to enter without really teaching you how to use it. I understand that there’s only so much depth one can go into in this type of course, but it makes it incredibly difficult to troubleshoot when the prompts they provide don’t work the way they’re supposed to.

### Discovering the power of loops

Once I finally got Vite working it was time for the fun part – setting up variables. Over the next few lessons, I set up variables for colors, fonts, font sizes, font weights, and spacing. Then I used the logic I learned in module two to loop through the variables and output utility classes for my CSS.

### Putting theory into practice

Once all the pieces were in place it was time to start the module project – building out a landing page from a Figma file using my new template.

This is the part I’d been looking forward to – actually writing CSS like a proper developer. I had to call on a lot of my previous CSS knowledge like flexbox, grid, and pseudo classes, but overall putting the site together was fairly painless.

One thing I struggled with was using utility classes in the HTML vs adding styles to my SCSS. I understand that in the long run it can lead to greater extensibility and thus more efficiency, but in the short term it seems cumbersome to add a utility class for color to each header, rather than just creating a separate class for headers in that color. It almost feels like going back to the very early days of the web before CSS existed when you had to add all your styles in the HTML itself.

I’ll confess I’m still a bit confused as to exactly when to use utility classes vs updating the CSS, and I also struggled a bit with the syntax. Because the template starts with abstracts in one SCSS file, then outputs them to create utility classes using loops and mixins, it takes a bit of reverse engineering to figure out what the syntax is for using the variables in the SCSS itself. I’m hoping this becomes clearer as time goes on.

Using utility classes for spacing also felt incredibly awkward to me at first. I suspect a lot of this had to with the fact that I didn’t plan out my divs as well as I should have before I started writing my HTML. It’s a pitfall I was aware of going in but knowing that and actually experiencing the pain of it are two very different things. That’s one of the reasons I was so excited for this project. Theory only takes you so far and it’s one thing to understand how these classes work and another thing entirely to actually write the code.

## What’s in store for module four

As excited as I was for module three, I think I’m even more excited for module four. During that module I’ll be using my templates and variables to put together design system tokens using CSS. I’m hoping to get into design systems engineering or something similar in the next few years, so I can’t wait to start playing with those building blocks!
