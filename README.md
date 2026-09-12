# Frontend Mentor - Bento Grid Solution

This is my solution to the [Bento Grid challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/bento-grid-RMydElrlOj).

The goal of this challenge was to recreate a responsive bento-style layout as closely as possible to the provided desktop and mobile designs using HTML and CSS.

## Overview

### The challenge

Users should be able to:

- View the optimal layout depending on their device's screen size.
- See the cards reorganize correctly between desktop and mobile layouts.

### Links

- Solution URL: Add your Frontend Mentor solution URL here
- Live Site URL: Add your deployed site URL here

## My process

### Built with

- Semantic HTML5
- CSS Grid
- Flexbox
- Media queries
- Responsive design
- Google Fonts - DM Sans

### What I learned

This challenge helped me understand CSS Grid much better, especially how to position items across different columns and rows to reproduce a more complex layout.

I also practiced combining Grid and Flexbox. Grid was useful for building the overall desktop structure, while Flexbox helped me align and distribute the content inside individual cards.

Another important part of the project was responsive design. The mobile version required more than simply shrinking the desktop layout. I had to change the grid to a single column, reorder the cards, and override several desktop-specific image sizes and spacing values.

Some examples of concepts I practiced were:

```css
.bento-grid {
  display: grid;
  grid-template-columns: repeat(4, 1fr);
}
```

and changing the layout for smaller screens:

```css
@media (max-width: 768px) {
  .bento-grid {
    grid-template-columns: 1fr;
    grid-template-rows: auto;
  }
}
```

### Challenges

One of the most difficult parts was understanding the structure of the desktop grid. Several cards span multiple rows or columns, so small changes to the grid could affect many other elements.

Another challenge was matching the proportions of the provided design. Since the reference is a static image, I had to experiment with spacing, image sizes, line heights, and card dimensions.

The mobile layout also required careful adjustments because some desktop styles, such as fixed image sizes and grid placement, had to be overridden inside the media query.

### Continued development

In future projects I want to improve:

- Planning the Grid structure before starting detailed styling.
- Writing responsive CSS with fewer one-off adjustments.
- Using fewer fixed values when a more flexible solution is possible.
- Organizing CSS so desktop and mobile overrides are easier to maintain.
- Becoming faster at identifying whether a visual issue comes from the grid itself or from the content inside a card.

## Author

- GitHub - [@marcosloll](https://github.com/marcosloll)
- Frontend Mentor - Add your Frontend Mentor profile here

## Acknowledgments

Thanks to Frontend Mentor for providing the challenge, design references, and assets.
