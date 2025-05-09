# Frontend Mentor - Social links profile solution

This is a solution to the [Social links profile challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/social-links-profile-UG32l9m6dQ).
## Table of contents

- [Overview](#overview)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [Continued development](#continued-development)

## Overview

### Screenshot

![](./src/images/Social%20links%20screenshot.png)

### Links

- [Link to Solution](https://www.frontendmentor.io/solutions/social-links-profile-using-scss-vite-zUHMo9Fud6)
- [Link to live site](https://networksentinel.github.io/Frontend-Mentor-Challenge---Social-links-profile/)

## My process

### Built with

- Semantic HTML5
- Sass/Scss - modular approach, mixins, variables
- Flexbox, fixed + relative units, clamp()
- [Vite](https://vite.dev/) - build tool

### What I learned

This was my first time actually using Sass/SCSS in a project, so basically everything was new to me — the symbols, the syntax, how mixins work, all of it.
I made a simple little mixin for handling fonts:

**(NOTE: I know the font shorthand property would be slightly more efficient, but I wanted to create my own version of it, just to exercise mixin creation/use.)**

```scss
@mixin font($font-size, $font-weight, $line-height: 150%, $letters-spacing: 0) {
  font-size: $font-size;
  font-weight: $font-weight;
  line-height: $line-height;
  letter-spacing: $letters-spacing;
}
```
It's nothing fancy, but it definitely made my life easier when setting up font styles. Here's how I used it:

```scss
.card__info-name {
  @include font($text-large, $text-weight-bold);
}

.card__info-place {
  @include font($text-small, $text-weight-bold);
  color: $green;
}
 .card__occupation {
    @include font($text-small, $text-weight-regular);
}
```

**Even though this was just a small challenge, I can already see how something like this could save a ton of repetitive code in bigger projects. My goal is to get into solid, professional habits early so things go smoother later — especially when working on larger projects or collaborating with others.**

Also, breaking the Sass files into separate modules made everything feel way more organized and readable. Definitely a habit I want to keep.

### Continued development

For my future projects, **I’ll be focusing on making Sass and Vite feel like second nature.** I want to get so comfortable with both that setting up a project with Git or diving into the code becomes automatic.

Commands like:
```
npm create vite@latest
npm install
npm run dev
npm run build
```

And with Sass:
- The modular approach (keeping things neat and organized)
- Working with mixins, functions, and variables
- Mastering nesting and other Sass features