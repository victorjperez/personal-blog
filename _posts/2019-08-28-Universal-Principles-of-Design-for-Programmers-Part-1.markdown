---
layout: Page
title: "Universal Principles of Design for Programmers: Part 1"
date: 2019-08-28 00:50:34 -0400
author: "Victor Perez"
categories: [tech]
image: "UPDFP_1.png"
---

During my third year of studying Computer Science, I wanted to vary up my schedule and add an English class to mix things up. I ended up taking Multimedia Writing, an upper-level English class intended for writers and designers. Despite being unnecessary for my degree, that class ended up being an incredibly valuable learning experience for me.

## Table Of Contents

- [What are Universal Principles of Design?](#what)
- [80/20 Rule](#80/20)
- [Aesthetic-Usability Effect](#Aesthetic-Usability)
- [Affordance](#Affordance)
- [Archetypes](#Archetypes)
- [Chunking](#Chunking)
- [Closure](#Closure)
- [Conclusion](#Conclusion)

### 🤷‍ What Are "Universal Principles of Design?" <a name="what"></a>

As the name suggests, **universal principles of design** are design principles that can be applied to many different disciplines. You could be organizing your house, making a poster, or even writing an operating system and use the same principles for all three. In this series, I'll be referencing the book _Universal Principles of Design_ by _William Lidwell_, an invaluable reference for design of any kind. In this case, however, I'll be taking specific ones and explaining how they relate to programming.

### 📏 80/20 Rule <a name="80/20"></a>

_A high percentage of effects in any large system are caused by a low percentage of variables._

- 80% of effort in a project is in the last 20% of work
- 80% of bugs are caused by 20% of the program
- 80% of application usage involves 20% of the functions

If you've ever worked on a large application of any kind, you've probably figured out by now that most users will never use every single feature. It's more likely the same handful of functions are used all the time, while the edge-case functions are rarely used, if at all. That's not to say that handling edge cases isn't important, but you can't let the scope of your application get out of control when working towards strict deadlines.

### 🖼 Aesthetic-Usability Effect<a name="Aesthetic-Usability"></a>

_Aesthetic designs are perceived as easier to use than less-aesthetic designs._

Ah yes, the dreaded programmer UI. At some point or another, we've all whipped up a quick GUI to test out the functionality of what we're working on. Sadly, that's not good enough when it comes to the final product. It doesn't matter how bug-free or perfect a piece of software is; if it's ugly, it's going to be used less. A designer can be just as important to a programmer when it comes to the success of your application.

### 🚪 Affordance<a name="Affordance"></a>

_A property in which the physical characteristics of an object or environment influence its function._

This one goes out to all the people who couldn't stop thinking about doors after reading _The Design of Everyday Things_. Things users interact with should make sense. A link should look like a link. A button should look like a button. Attention to detail is important, and the less time a user spends thinking about your design, the less you need to explain it.

### 💾 Archetypes<a name="Archetypes"></a>

_Universal patterns of theme and form resulting from innate biases or dispositions._

Naming remains an incredibly important part of programming. So much so that conventions and style guides are written to keep everyone on the same page. You can also use archetypes to make complex functions easier to understand in code. For example: say you have a program that stores a list of students, and a function that removes students with a GPA under 2.0. Naming your function `removeStudents()` is too ambiguous. You could try something longer such as `removeStudentsUnderGPALimit()`, which is unambiguous, but that reduces readability. A good solution could be `expellForGPA()`, as expelling is a real-world pattern that most people will be familiar with.

### 🎒 Chunking<a name="Chunking"></a>

_A technique of combining many units of information into a limited number of units or chunks, so that the information is easier to process and remember._

Information overload can be a big issue when displaying necessary data to both users and collaborators. A classic example I see is when beginners first learn about commenting code and then proceed to fill the beginning of every file with a large multi-line comment explaining the purpose of every object, variable, and function. Large walls of text often end up being ignored, so break up your comments when you can.

### 🧩 Closure<a name="Closure"></a>

_A tendency to perceive a set of individual elements as a single, recognizable pattern, rather than multiple, individual elements._

This is a different definition of closure than the programming one you're probably used to seeing. A closure in design refers to how our brains naturally look for patterns. In UI, you can leverage this to simplify the amount of information displayed on the screen (for both performance and readability's sake). In code, you can use the thought process behind this principle to make things more readable. Take JavaScript's `Array.prototype.map()` for example.

```javascript
let list = [1, 2, 3];
for (let item = 0; item < list.length; item++) {
  list[item] = list[item] * 2;
}
```

While iterating through arrays is trivial, it still takes mental overhead when reading to ensure that everything is behaving as expected. We can simplify this using `Array.prototype.map()`

```javascript
let list = [1, 2, 3];
let doubledList = list.map(item => item * 2);
```

Once you learn how this pattern works, your mind will subconsciously tell you "an action is being taken on every item in this list." Under the hood, it might just be a for loop, but we don't have to think about it.

### 🙇‍ Conclusion<a name="Conclusion"></a>

This concludes this part of _Universal Principles of Design for Programmers_! Hopefully these principles made you think about what design can do for you. More principles to come!
