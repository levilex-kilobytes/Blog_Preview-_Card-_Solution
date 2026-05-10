# Frontend Mentor - Blog Preview Card Solution

This is a solution to the [Blog preview card challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/blog-preview-card-ckPaj01IcS).

## Table of contents

- [Overview](#overview)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [Continued development](#continued-development)
  - [Useful resources](#useful-resources)
  - [AI Collaboration](#ai-collaboration)
- [Author](#author)
- [Acknowledgments](#acknowledgments)

## Overview

### Screenshot

![Screenshot of Blog Preview Card solution](./screenshot.jpg)

### Links

- Solution URL: https://github.com/levilex-kilobytes/Blog_Preview-_Card-_Solution
- Live Site URL: https://blog-preview-card-solution-umber.vercel.app/

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- BEM naming convention
- Flexbox
- Mobile-first workflow
- Google Fonts (Figtree)

### What I learned

I learned how to apply BEM naming convention properly, separating
blocks, elements, and modifiers clearly:

```html
<article class="card">
  <div class="card__body">
    <h1 class="card__title">HTML & CSS foundations</h1>
  </div>
</article>
```

I also learned how to use `clamp()` to make font sizes and spacing
responsive without relying on many media queries:

```css
--fs-title: clamp(1.1rem, 3vw, 1.25rem);
```

And how to support users who prefer reduced motion:

```css
@media (prefers-reduced-motion: reduce) {
  .card {
    transition: none;
  }
}
```

### Continued development

- CSS Grid for more complex layouts
- Better accessibility practices (ARIA labels)
- Learning `container queries` as an alternative to media queries
- Improving Git workflow from the start of each project

### Useful resources

- [MDN - clamp()](https://developer.mozilla.org/en-US/docs/Web/CSS/clamp) - Helped me understand how to use clamp() for fluid typography.
- [BEM Methodology](https://getbem.com/) - Great reference for BEM naming.
- [CSS Tricks - Flexbox](https://css-tricks.com/snippets/css/a-guide-to-flexbox/) - Used for centering the card on the page.
- [prefers-reduced-motion](https://developer.mozilla.org/en-US/docs/Web/CSS/@media/prefers-reduced-motion) - Helped me handle motion accessibility correctly.

### AI Collaboration

I used **Claude (Anthropic)** throughout this project:

- **BEM structure** — Claude helped refactor the original HTML to use
  proper BEM naming across all elements.
- **Accessibility fixes** — Claude identified and fixed issues like
  missing `<h1>`, reduced motion support, and focus states.
- **Responsive CSS** — Claude helped replace fixed `px` values with
  `clamp()`, `min()`, and `rem` units for better responsiveness.
- **Git workflow** — Claude helped fix repeated `git push` errors
  caused by skipping `git add .` before committing.

What worked well: Getting step-by-step explanations of _why_ each
fix was needed, not just _what_ to change.

## Author

- Frontend Mentor - levilex-kilobytes(https://www.frontendmentor.io/profile/levilex-kilobytes)
- Twitter - itzlevi005(https://x.com/Itzlevi005)

## Acknowledgments

Thanks to [Frontend Mentor](https://www.frontendmentor.io) for this
challenge and to Claude (Anthropic) for guidance on accessibility,
BEM, and responsive CSS best practices.
