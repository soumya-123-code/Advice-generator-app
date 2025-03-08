# Advice Generator App

## Welcome! 👋

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [How to setup the project](#how-to-setup-the-project)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [Continued development](#continued-development)
  - [Useful resources](#useful-resources)
- [Author](#author)
- [Acknowledgments](#acknowledgments)

## Overview

### The challenge

Users should be able to:

- View the optimal layout for the app depending on their device's screen size
- See hover states for all interactive elements on the page
- Generate a new piece of advice by clicking the dice icon

### How to setup the project

To set up the project locally, follow these steps:

1. Clone the repository using GitHub Desktop or Git Bash:
   ```bash
   git clone https://github.com/soumya-123-code/Advice-generator-app.git
   ```
2. Open the project folder in your code editor.
3. Run the project using a live server extension or deploy it using Netlify, Vercel, or another web hosting and deployment service.

### Screenshot

![Design preview for the Advice generator app coding challenge](./design/active-states.jpg)

### Links

- Solution URL: [Link to this repo](https://github.com/soumya-123-code/Advice-generator-app)
- Live Site URL: [Advice Generator](https://free-advice-generator-frontend.netlify.app)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- Promises, async await
- Vanilla JavaScript

You will find all the required assets in the `/images` folder. The assets are already optimized.

There is also a `style-guide.md` file containing the information you'll need, such as color palette and fonts.

### What I learned

This project can be a great teacher to someone who is not well versed with the concept of working with fetch and async await syntax of JavaScript, which can be a pain for beginners when told to implement on their own.

<b>js = proud of this function</b>

```js
const fetchAdvice = async () => {
    title.style.marginBottom = "6rem";
    dualRing.classList.remove("disabled");
    ctaBtn.classList.add("disabled");
    isDisabled = true;
    setTimeout(async () => {
        const response = await fetch("https://api.adviceslip.com/advice");
        const data = await response.json();
        const { id, advice } = data.slip;
        adviceIdSpan.innerHTML = id;
        quoteDiv.innerHTML = `“${advice}”`;
        dualRing.classList.add("disabled");
        title.style.marginBottom = "0";
    }, 500);
    setTimeout(() => {
        ctaBtn.classList.remove("disabled");
        isDisabled = false;
    }, 2000);
};
```

### Continued development

The continuously learning journey of a programmer never ends. This project made me realize that there are many concepts that I need to work upon, including fundamentals like flexbox and its properties, to more complex concepts like working with fetch and async await in JavaScript. These areas are some that I think I need to work more upon in the upcoming future as they highlight some of the most significant regions of web development that are important for every developer to know of.

These key points mentioned here will help me grow accountable and consistent towards improving at writing good quality code and becoming a successful full-stack developer one day.

### Useful resources

- [Harkirat Singh course notes](https://github.com/soumya-123-code/harkirat-singh-course_code_and_notes) - I have added notes of all lectures along with code and lecture insights of all weeks along with bonus lectures to help you all as much as I can.
- [My development code and notes](https://github.com/soumya-123-code/cwh-web-dev-playlist_code_and_notes) - These are my notes that I made while working on my development skills in initial days and did these courses. Make sure to star the repository if you like it. ✨💫
- [MDN Documentation](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/async_function) - This is an amazing article that helped me finally understand promises, async, and await syntax. I'd recommend it to anyone still learning this concept.

## Author

<b><strong>Soumya Ranjan Nayak</strong></b>
- Portfolio - [Soumya Ranjan Nayak](https://soumya-123-code.github.io/itsmesoumya)
- GitHub - [@soumya-123-code](https://github.com/soumya-123-code/)
- LinkedIn - [Soumya Ranjan Nayak](www.linkedin.com/in/soumya-ranjan-nayak-50069a15a)

## Acknowledgments

I feel like the solutions provided on the website and the continuous doubt solving by industry experts on Discord for free is something that is unmatched by anyone else and needs to be acknowledged for their efforts in improving me as a developer by suggesting the best practices in your respective tech stack.

## Got feedback for me?

I love receiving feedback! I am always looking to improve my code and take up new innovative ideas to work upon. So if you have anything you'd like to mention, please email 'hi' at soumya050794@gmail.com.

If you liked this project, make sure to spread the word and share it with all your friends.

**Have fun reading advice and succeeding in life!** ☺️🚀

