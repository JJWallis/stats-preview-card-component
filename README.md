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

## Overview

### The challenge

Your users should be able to:

-  View the optimal layout depending on their device's screen size

### Screenshot

![](./screenshot.png)

### Links

-  Live Site URL: https://stats-preview-component-jjw.netlify.app/

## My process

### Built with

-  Semantic HTML5 markup
-  Flexbox
-  Mobile-first workflow

### What I learned

```html
<ul>
   <li>
      <span>10k+</span>
      <span>companies</span>
   </li>
   ...
</ul>
```

This was my first project using an unordered list as a flex container instead of a more traditional div, which stylistically makes sense as technically it's still a block-level element. The child's list items also provide a convenient and semantic wrapper to act as the flex item containers.

```html
<h1>Get <strong>insights</strong> that help your business grow.</h1>
```

This project further provided some great practice for experimenting with different inline semantic elements, as well as the effect they each had on the layout. Although I decided to use a `<strong>` tag to place additional emphasis on content within the title, I equally realise that using a `<span>` tag just to style a word differently is also perfectly valid, since the whole heading would still be read aloud with the same level of importance.

```css
.background-container {
   background: rgb(170, 92, 219) url('/images/image-header-mobile.jpg') no-repeat
      center;
   background-blend-mode: multiply;
   min-height: 300px;
}
```

The blending of a background image with its fallback colour in case the image becomes unavailable, provides a really nice effect on top of the original asset and can help it 'blend' into the original design. Here I used the `multiply` value to darken the asset and enable it to fit in with the very dark blue background colour.

```css
.wrapper {
   min-height: 400px;
   border-radius: 5px;
   overflow: hidden;
}
```

I learned how to change the border-radius of the parent wrapper whilst applying an `overflow: hidden;` to prevent all child content from escaping underneath and ruining its curve. This was a much more efficient method than my original solution, where I manually changed each specific corner at different viewports.

Finally, I was able to apply a `min-height` to the flex-item and parent wrapper housing the background image in order to prevent it from collapsing. This was because it wasn't housing any content in the DOM, and since a background image is only for decorative purposes, it won't be announced by any assistive technology.

### Continued development

### Useful resources

-  [CSS Blending Modes](https://www.youtube.com/watch?v=-c94pr41jaI&ab_channel=KevinPowell) - This video helped me gain more confidence in experimenting with different blend modes alongside different styles of images. In this project I used the 'multiply' value to create a darkened effect over the primary background image.

## Author

-  Website - [Joshua Jameson-Wallis](https://www.joshuajamesonwallis.com/)
-  Linkedin - [Joshua Jameson-Wallis](https://www.linkedin.com/in/joshua-jameson-wallis/)
