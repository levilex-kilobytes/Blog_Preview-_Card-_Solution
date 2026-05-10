# Frontend Mentor - Blog Preview Card Solution

This is a solution to the [Blog preview card challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/blog-preview-card-ckPaj01IcS). Frontend Mentor challenges help you improve your coding skills by building realistic projects.

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

This project helped me understand **CSS Custom Properties (Variables)** and how they make code easier to maintain. Instead of repeating the same color or value everywhere, I define it once in `:root` and reuse it throughout the stylesheet.

```css
:root {
  --color-yellow: #f4d03f;
  --shadow: 4px 4px 0px var(--color-black);
}

.card {
  box-shadow: var(--shadow);
}

.card__tag {
  background-color: var(--color-yellow);
}
```

I also practiced **BEM naming convention** to keep my HTML and CSS organized:

```html
<article class="card">
  <div class="card__body">
    <h2 class="card__title">HTML & CSS foundations</h2>
    <p class="card__text">These languages are the backbone...</p>
  </div>
</article>
```

And I learned how to add **hover and focus states** for accessibility:

```css
.card__title-link:hover .card__title {
  color: var(--color-yellow);
}

a:focus-visible {
  outline: 2px solid var(--color-black);
  outline-offset: 3px;
}
```

### Continued development

In future projects I want to focus on:

- Getting more comfortable with CSS Grid for complex layouts
- Learning more about accessibility (ARIA labels, keyboard navigation)
- Practicing animations and transitions for smoother hover effects
- Understanding when to use `rem` vs `px` for spacing and font sizes

### Useful resources

- [MDN - CSS Custom Properties](https://developer.mozilla.org/en-US/docs/Web/CSS/Using_CSS_custom_properties) - Helped me understand how CSS variables work and why `:root` is used.
- [BEM Methodology](https://getbem.com/) - Great reference for understanding Block, Element, Modifier naming.
- [CSS Tricks - Flexbox Guide](https://css-tricks.com/snippets/css/a-guide-to-flexbox/) - Used this to center the card perfectly on the page.

### AI Collaboration

- **Debugging** — When my CSS wasn't being applied, Claude helped me identify that the file path and file name had to match exactly.

## Author

- Frontend Mentor - levilex-kilobytes(https://www.frontendmentor.io/profile/levilex-kilobytes)
- Twitter - itzlevi005(https://x.com/Itzlevi005)

## Acknowledgments

Thanks to [Frontend Mentor](https://www.frontendmentor.io) for this challenge.
