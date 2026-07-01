# Frontend Mentor - Blog preview card solution

This is a solution to the [Blog preview card challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/blog-preview-card-ckPaj01IcS). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [Continued development](#continued-development)
  - [AI Collaboration](#ai-collaboration)
- [Author](#author)

## Overview

### The challenge

Users should be able to:

- See hover and focus states for all interactive elements on the page

### Screenshot

![](./assets\images\screenshot.png)

### Links

- Solution URL: [GitHub solution URL](https://github.com/bessoAgustin/blog-preview-card.git)
- Live Site URL: [GitHub Pages live site URL](https://bessoagustin.github.io/blog-preview-card/)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- Mobile-first workflow

### What I learned

This project has helped me deepen my understanding in how CSS Flexbox attributes work and how powerful they are at controlling the design flow. I also commited myselt to thinking with a "mobile-first" mindset at all times, being weary of responsiveness issues to guarantee a clean and easy experience independently of device sizes.

I used box sizing for the first time to avoid the padding of my card to be added to my container's `<div>` width. 

```css
*{
  box-sizing: border-box;
}
```

Regarding responsiveness:

- I used <em>'rem'</em> accordingly for relative sizing
- <em>'max-width'</em> instead of simply 'width'
- <em>'overflow-wrap'</em> to prevent cases like the word "foundations" in the `<h2>` to break the structure in small screens.


```css
.container {
  display: flex;
  flex-direction: column;
  text-wrap: wrap;
  overflow-wrap: break-word; 
  margin-top: auto;
  margin-bottom: auto;
  background-color: hsl(210, 46%, 95%);
  max-width: 24rem;
  width: 90%;
  height:fit-content;
  border: solid 1px hsl(0, 0%, 7%);
  box-shadow: 8px 8px hsl(0, 0%, 0%);
  border-radius: 20px;
  padding: 1.5rem;
  gap: 1.5rem;
  background-color:hsl(0, 0%, 100%);
}
```
I also installed the <strong>'px to rem'</strong> extension in VSCode to help me convert px values to rem values, which was very effective for this project.

Finally, it was very interesting to learn about the `padding-bottom` and `padding-block-end` attribute differences, which are very similar but have different behaviors. I used `padding-block-end` in the `<body>` tag to ensure that the padding would be applied correctly regardless of the writing mode.

```css
padding-block-end: 1.5rem;
```

### Continued development

In the future, I would like to continue improving my CSS skills, especially in the area of Flexbox and Grid. I also want to learn more about accessibility and how to make my websites more inclusive for all users, before moving on to more advanced topics like JavaScript and React.

### AI Collaboration

I used Gemini throughout the project to help me with debugging and brainstorming solutions. It was particularly helpful in identifying issues with my CSS and suggesting alternative approaches to achieve the desired layout. Given the instructions in the `AGENTS.md` file, Gemini was able to provide guidance without giving me the answers directly, which helped me learn and improve my skills.

## Author

- GitHub - [@bessoAgustin](https://github.com/bessoAgustin)
- Frontend Mentor - [@bessoAgustin](https://www.frontendmentor.io/profile/bessoAgustin)