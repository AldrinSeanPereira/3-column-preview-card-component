# Frontend Mentor - 3-column preview card component solution

This is a solution to the [3-column preview card component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/3column-preview-card-component-pH92eAR2-). Their challenges help you improve your coding skills by building realistic projects. 

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

**Note: Delete this note and update the table of contents based on what sections you keep.**

## Overview

### The challenge

Users should be able to:

- View the optimal layout depending on their device's screen size
- See hover states for interactive elements

### Screenshot

![3-column preview card component](3-column-preview-card-component.png)

### Links

- Solution URL: [link](https://github.com/AldrinSeanPereira/3-column-preview-card-component)
- Live Site URL: [link](https://gleaming-froyo-5aa2b4.netlify.app/)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- Mobile-first workflow

### What I learned

This project taught me:
- Mobile first workflow
- working with SVGs
- sizing the `body` and `main` in CSS
- use of `flex-grow`

I really am amazed by the CSS I have made but this snippet is the masterpiece of the whole thing:

```css
body {
    min-height: 100vh; 
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    position: relative;
}

main {
    width: 100%;
    height: 100%;
    flex-grow: 1;
    display: flex;
    justify-content: center;
    align-items: center;
    flex-wrap: wrap;
}
```
I'm saving this particular piece of advice by `Alex K Marshall` here because it is so helpful to me:

- Never set a width on the `body`. And percentage heights don't work in a very intuitive way, so is usually not what you want.

- **Set the `body` to `min-height: 100vh` and then the `body` will fill the screen.**

(NOTE: Next I made `main` to have 100% height and width of the container which is `body`)

- Inside the `body` you have `main` and `footer`, we want `footer` at the bottom and `main` to take up the rest of the space. 

- So, you can make `body` a `display: flex` and `flex-direction: column`. 

- And then give `main` a `flex-grow: 1` which means "grow to fill any available space". Since footer doesn't have that, `main` will take up the full height of the screen (the `body` height) plus any space that the `footer` takes


### Continued development

Will do more projects from the `challenge roadmaps` in the Frontend Mentor discord

### Useful resources

- [Interneting is hard](https://internetingishard.netlify.app/html-and-css/index.html) 
 
  - A *golden resource* to have. Beautiful images and explanations!

  - I learned so much about starting a project, responsive web design,
relative and absolute URL paths.
- [About Flex Grow](https://developer.mozilla.org/en-US/docs/Web/CSS/flex-grow) 
  - When Alex told me about the flex grow property, I used this resource to learn more about it.

## Author

- LinkedIn - [Aldrin Sean Pereira](https://www.linkedin.com/in/aldrinseanpereira/)
- Frontend Mentor - [@AldrinSeanPereira](https://www.frontendmentor.io/profile/yourusername)
- GitHub - [@AldrinSeanPereira](https://www.frontendmentor.io/profile/AldrinSeanPereira)


## Acknowledgments

Thank you to the support team on the Frontend Mentor Discord server especially Chamu, Alex K Marshall and Grace Snow. You are awesome!!
