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
- [Author](#author)

## Overview

### The challenge

Users should be able to:

- View the optimal layout for the component depending on their device's screen size
- See hover states for all interactive elements on the page
- Hide/Show the answer to a question when the question is clicked

### Screenshot

![](.\screenshots\screenshot_desktop.png)


### Links

- Solution URL: [Add solution URL here](https://your-solution-url.com)
- Live Site URL: [Add live site URL here](https://your-live-site-url.com)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- CSS Grid
- Mobile-first workflow
- VScode

### My process and What I learned

I set out to finish this challenge withouth using javascript. I had to think a bit about the response bit with the different images I had to change and also the accordion. But the solution was pretty straigt forward using @media and css background image. For the accordion I used details, summary. See code snippets below. To get rid of the default bullet points you need a list-style of none and the marker pseudo class to be display none.

My workflow was using a mobile first approach and then change the bits that was needed. 

Added subtle animation to the arrows.

```html
<details>
  <summary><h3>How many team members can I invite?</h3></summary>
  <p>You can invite up to 2 additional users on the Free plan. There is no limit on team members for the Premium plan.</p>
</details>
```
```css
details > summary {
  display: inline-block;
  position: relative;
  cursor: pointer;
  list-style: none;
  margin-right: 4em;
  color: var(--ntxt-Dark-grayish-blue);
}
details > summary::-webkit-details-marker {
  display: none;
}
```


### Continued development

I started out using mainly Flexbox for this challenge, but ended up rewritting it for Grid. It made it easier for sizing and positioning. Need to learn more to optimize and find som good practices when to use what. 


## Author

- Frontend Mentor - [@spaceflake](https://www.frontendmentor.io/profile/spaceflake)
- Twitter - [@spaceflake1](https://www.twitter.com/spaceflake1)
- Facebook - [@tomasfridekrans](https://www.facebook.com/tomasfridekrans)

