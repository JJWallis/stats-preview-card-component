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
<ul>
   <li>
      <span>10k+</span>
      <span>companies</span>
   </li>
   ...
</ul>
```

This was my first project using an un-ordered list as a flex-container instead of the traditional div, which stylistically makes sense as technically it's a block-level container. The child list-items also provide convenient flex-item containers to control using flex's algorithm.

```html
<h1>Get <strong>insights</strong> that help your business grow.</h1>
```

This project further provided some great practice for experimenting with different inline semantic elements, and the effect they each had on the layout. Although I decided to use a strong tag to place additional emphasis on content within the title, I equally realise that using a `<span>` tag just to style a word differently is also perfectly valid, since the whole heading would be read aloud with the same level of importance.

```css
.background-container {
   background: rgb(170, 92, 219) url('/images/image-header-mobile.jpg') no-repeat
      center;
   background-blend-mode: multiply;
   min-height: 300px;
}
```

The blending of a background image with its fallback colour (in case the image becomes unavailable) provides a really nice effect to to the original asset, and can help it 'blend' into the design created for the project. Here I used the multiply value to darken the asset, which looked much closer to the design mockup provided and enabled it to fit in with the very dark blue background colour.

```css
.wrapper {
   min-height: 400px;
   border-radius: 5px;
   overflow: hidden;
}
```

Additionally, I learned how to change the border-radius of the parent wrapper whilst applying an `overflow: hidden;` to prevent all child content from escaping and ruining the curve. This was a much more efficient method than my original solution, where I manually changed each specific corner at different media breakpoints.

Finally, I was able to apply a min-height to the flex-item (and parent wrapper) housing the background image in order to prevent it from collapsing. This was because it wasn't housing any content in the DOM, as a background image is only for decorative purposes and as such will not be announced by any assistive technology.

### Continued development

### Useful resources

-  [CSS Blending Modes](https://www.youtube.com/watch?v=-c94pr41jaI&ab_channel=KevinPowell) - This video helped me gain more confidence in experimenting with different blend modes alongside different styles of images, where in this project I used the 'multiply' value to create a darkened effect over the primary background image.

## Author

-  Website - [Joshua Jameson-Wallis](https://joshuajamesonwallis.com)
-  Linkedin - [Joshua Jameson-Wallis]()

## Acknowledgments

I have included a copy of the solution that I used for this project in the repo. This helped me with the wrapping behaviour of each statistic, which wasn't originally working because I was restricting the width of the flex container that was causing my flex-items to not wrap when desired.

Testing, testing, testing

Testing, testing, testing
