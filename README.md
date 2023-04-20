# Frontend Mentor - Product preview card component solution

This is a solution to the [Product preview card component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/product-preview-card-component-GO7UmttRfa). Frontend Mentor challenges help you improve your coding skills by building realistic projects.

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

- View the optimal layout depending on their device's screen size
- See hover and focus states for interactive elements

### Screenshot

![](./screenshot.png)

### Links

- Solution URL: [Github](https://github.com/Jun-Ueno/product-preview-card-component)
- Live Site URL: [Live](https://jun-ueno.github.io/product-preview-card-component/)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- CSS Grid

### What I learned

You would think that a container with rounded corners would apply the corners to child elements, but that's not always the case. The perfume image had to have different corner applied in desktop and mobile views. Also, I found using background images instead of images worked better for this layout.

```css
.image {
  background-image: url('./images/image-product-desktop.jpg');
  background-size: cover;
  background-position: center center;
  border-radius: 0.75rem 0 0 0.75rem;
}
@media screen and (max-width: 480px) {
  .image {
    background-image: url('./images/image-product-mobile.jpg');
    border-radius: 0.75rem 0.75rem 0 0;
  }
}
```

### Useful resources

- [A Complete Guide to CSS Grid](https://css-tricks.com/snippets/css/complete-guide-grid/) - Cheat sheet for understanding CSS grid. A must-bookmark.
- [A Complete Guide to Flexbox](https://css-tricks.com/snippets/css/a-guide-to-flexbox/) - Makes CSS flexbox easy to understand.

## Author

- Frontend Mentor - [@Jun-Ueno](https://www.frontendmentor.io/profile/Jun-Ueno)
- LinkedIn - [@jun-ueno-5a558163](https://www.linkedin.com/in/jun-ueno-5a558163/)
