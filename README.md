# Skillcrush project - Single-page developer portfolio solution

As part of my Front-End Developer Track at Skillcrush, I completed this project which enabled me to acquire additional front-end development skills.

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [Useful resources](#useful-resources)
- [Author](#author)

## Overview

### The challenge

Users should be able to:

- Click on an invite button to add a new guest to a list of attendees
- See the total number of guests attending
- Be alerted when the guest list is full
- Click on an assign button to randomly assign potluck items to each guest on the list, and display the assigned items in a separate list.

### Screenshot

![](./img/project-screenshot.jpg)

### Links

- Live Site URL: [Add live site URL here](https://your-live-site-url.com)

## My process

### Built with

- Flexbox
- Mobile-first workflow
- JavaScript


### What I learned

Working on this project I could learn:
- how to use arrays to store and manipulate data.
- how to generate random numbers using Math.random() and use them to select items from an array.
- how to use loops to iterate over arrays and perform operations on their contents.

Here are some code snippets for the things mentioned earlier:

```js 
{
//using arrays to store and manipulate data
const potluckItems = [
  "potato salad",
  "hummus",
  "cookies",
  "fruit",
  "tomato and mozzarella caprese skewers",
  "chicken salad spring rolls",
  "sandwiches",
  "cucumber noodles",
  "salsa",
  "icebox cake",
  "peach tarts",
  "ice-cream"
];

const allGuests = document.querySelectorAll(".guest-list li");

//using Math.random()
let randomPotluckIndex = Math.floor(Math.random() * potluckItems.length);
let randomPotluckItem = potluckItems[randomPotluckIndex];

//using loops to iterate over arrays
for (let guest of allGuests) {
  let randomPotluckIndex = Math.floor(Math.random() * potluckItems.length);
  let randomPotluckItem = potluckItems[randomPotluckIndex];

  let listItem = document.createElement("li");
  listItem.innerText = `${guest.innerText} is bringing ${randomPotluckItem}.`;
  assignedItems.append(listItem);

  potluckItems.splice(randomPotluckIndex, 1);
}
}
```

### Useful resources

- [Resource 1](https://javascript.info/array) - This helped me for getting a detailed guide to working with arrays in JavaScript. It covers topics like creating arrays, adding and removing elements, and using array methods like forEach and map
- [Resource 2](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array) - This is an amazing article which helped me arrays in JavaScript. It covers everything from creating and initializing arrays to using array methods to manipulate their contents.

## Author

- LinkedIn - [Doina Leovchin](https://www.linkedin.com/in/doinaleovchindeveloper/)
