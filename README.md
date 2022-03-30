# Frontend Mentor - FAQ accordion card solution

This is a solution to the [FAQ accordion card challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/faq-accordion-card-XlyjD0Oam). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
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

- View the optimal layout for the component depending on their device's screen size
- See hover states for all interactive elements on the page
- Hide/Show the answer to a question when the question is clicked

### Screenshot

![](./img/screenshot.jpeg)

### Links

- Live Site URL: [See the demo on Github Pages](https://jimi-s-frontend-mentor-cs.github.io/FAQ-accordion-card/)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- CSS Grid
- Mobile-first workflow
- SASS

### What I learned

I learned the use of ```<summary>``` and ```<detail>``` tags for creating the FAQ section. I also learned how to style them to fit the desired result


```css
summary {
    cursor: pointer;
    list-style-type: none;

    &::after {
        content: url("../img/icon-arrow-down.svg");
        float: right;
    }

    &:hover,
    &:active {
        color: $clrTextPrimarySoftRed;
    }
}

&[open] {
    summary {
        &::after {
            content: url("../img/icon-arrow-down.svg");
            transform: rotateX(180deg);
        }
    }
}
```

### Continued development

I had some issues with the image overlapping the main area, and there are still issues you can find when resizing at certain resolutions. I definitively need to improve on this area.

### Useful resources

- [This Stack Overflow Answer](https://stackoverflow.com/a/10813665/2695796) - This helped me customize the arrow for the questions
- [Kevin Powell](https://www.youtube.com/kepowob) - This amazing guy helped me A TON getting me back into Web Development, refreshing by knowledge and also teaching me new stuffs and tricks (especially with CSS and flexbox).

## Author

- Frontend Mentor - [@JimiIT92](https://www.frontendmentor.io/profile/JimiIT92)

## Acknowledgments

Big shoutout to [Konrad Rudolph](https://stackoverflow.com/a/10813665/2695796) and [Kevin Powell](https://www.youtube.com/kepowob) for sharing their solutions and resources to the public, so other developers like me can learn new stuff!