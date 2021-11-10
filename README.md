# Frontend Mentor - Stats preview card component solution

This is a solution to the [Stats preview card component challenge](linkhttps://www.frontendmentor.io/challenges/stats-preview-card-component-8JqbgoU62) on Frontend Mentor

## Table of contents

-  [Overview](#overview)
   -  [The challenge](#the-challenge)
   -  [Screenshot](#screenshot)
   -  [Links](#links)
-  [My process](#my-process)
   -  [Built with](#built-with)
   -  [What I learned](#what-i-learned)
   -  [Continued development](#continued-development)
   -  [Useful resources](#useful-resources)
-  [Author](#author)
-  [Acknowledgments](#acknowledgments)

## Overview

### The challenge

Your users should be able to:

-  View the optimal layout depending on their device's screen size

### Screenshot

![](./Screenshot.png)

### Links

-  Live Site URL:

## My process

### Built with

-  Semantic HTML5 markup
-  Flexbox
-  Mobile-first workflow

### What I learned

```html
<h1>Get <strong>insights</strong> that help your business grow.</h1>

<ul>
   <li>
      <span>10k+</span>
      <span>companies</span>
   </li>
   ...
</ul>
```

This was my first project using an un-ordered list as a flex-container instead of the traditional div, which stylistically makes sense as technically it's a block-level container. The child list-items also provide convenient flex-item containers to control using flex's algorithm.

```css
.background-container {
   background: rgb(170, 92, 219) url('/images/image-header-mobile.jpg') no-repeat
      center;
   background-blend-mode: multiply;
}
```

### Continued development

### Useful resources

-  [CSS Blending Modes](https://www.youtube.com/watch?v=-c94pr41jaI&ab_channel=KevinPowell) - This video helped me gain more confidence in experimenting with different blend modes alongside different styles of images, where in this project I used the 'multiply' value to create a darkened effect over the primary background image.

## Author

-  Website - [Joshua Jameson-Wallis](https://joshuajamesonwallis.com)
-  Linkedin - [Joshua Jameson-Wallis]()

## Acknowledgments

I have included a copy of the solution that I used for this project in the repo. This helped me with the wrapping behaviour of each statistic, which wasn't originally working because I was restricting the width of the flex container that was causing my flex-items to not wrap when desired.

###### TODO

HTML:

Good practice for using inline semantic tags within <p>'s - strong (instead of a <span> - maybe not appropiate as just style - screenreaders read in diff way which wouldn't make sense) | <section> vs <div>

CSS:

Background-blend-mode + fallback bg colour with img (1st time) |

Border-radius shorthand vs all 4 corners individually + overflow hidden (no need to change dynamically when breakpoint hits)

Min-height - fluid + forced to see img in div with no content
