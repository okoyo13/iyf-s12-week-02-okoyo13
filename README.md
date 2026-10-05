# IYF S12 · Week 02 · Lessons 3 & 4

This repository contains my Lesson 3 and Lesson 4 work for the IYF S12 program,
focused on CSS foundations and responsive layout. Lesson 3 covered base
styling, the box model, a modular typography system, and a color scheme built
with custom properties. Lesson 4 builds on that foundation with Flexbox, CSS
Grid, mobile-first responsive design, and final polish for accessibility and
interaction.

## Project Structure

The repository holds one responsive portfolio page at the root, plus three
self-contained practice folders that each demonstrate specific CSS concepts.
At the root, `index.html` is the portfolio home and pulls its styles from
`styles.css`, which now includes the design tokens from Lesson 3 plus the
flex, grid, and responsive rules from Lesson 4. Inside `flexbox-practice/`,
you'll find a page that demonstrates a responsive navigation bar, a wrapping
card row, and a three-column footer. Inside `grid-practice/`, there's a page
that shows a three-column photo gallery, a magazine-style layout using
`grid-template-areas`, and a responsive project-cards grid. The
`box-model-practice/` and `typography-system/` folders from Lesson 3 remain
unchanged and are still viewable on their own.

## What Each Lesson Covers

Lesson 3 started with CSS setup — linking an external stylesheet, resetting
defaults, and setting a 16px root size with a 1.6 line-height. From there, the
box-model practice folder visualizes content, padding, border, and margin,
then debugs a classic `content-box` width bug, and finally builds a 300px card
with precise internal spacing. The typography system pairs Montserrat for
headings with Open Sans for body text and runs a modular scale from 12px up
to 36px using custom properties. The color scheme defines a primary brand
blue, an amber accent, plus light and dark variants, muted text, surfaces,
and borders — all as tokens so any value can be changed in one place.

Lesson 4 moves into layout. The Flexbox practice page covers a navigation bar
with the logo left and links right, a row of three equal-height cards that
wrap on smaller screens, and a footer split into three columns above a
centered copyright line. The Grid practice page covers a three-column photo
gallery with consistent gaps, a magazine layout that uses named grid areas to
span a header and footer across the full width with a sidebar and main column
in between, and a responsive projects grid that drops from three columns on
desktop to two on tablet to one on mobile. The main portfolio page itself
was rebuilt mobile-first: base styles target phones, then media queries at
768px, 1024px, and 1280px layer on tablet and desktop treatments. Navigation
switches from a CSS-only hamburger menu on mobile to a horizontal menu on
desktop, hero content stacks on mobile and splits on desktop, and every
interactive element has hover, focus, and transition states.

## Getting Started

There's nothing to install. You can open any `index.html` directly in a
browser, or — for consistent font loading and clean URLs — run
`python3 -m http.server 8000` from the project root. Then visit
`http://localhost:8000/` for the portfolio home,
`http://localhost:8000/flexbox-practice/` for the Flexbox exercises, or
`http://localhost:8000/grid-practice/` for the Grid exercises.

## Concepts Practiced

Across both lessons, the work touches most CSS fundamentals: global resets
and `border-box` sizing, the box model and how padding and borders interact
with width, modular type scales, CSS custom properties as design tokens,
font pairing, color systems with variants, Flexbox for one-dimensional
layout, CSS Grid for two-dimensional layout, named grid areas, responsive
images, mobile-first media queries, CSS-only hamburger navigation, hover and
focus states for accessibility, and smooth transitions on interactive
elements. Everything is vanilla HTML and CSS — no frameworks, no build step.

## References

MDN Web Docs were the primary reference, especially the CSS First Steps and
Box Model pages. For layout, I used the CSS-Tricks Guide to Flexbox and Guide
to Grid, and I completed Flexbox Froggy and Grid Garden before starting
Lesson 4. The type scale came from the online Type Scale Calculator, and the
color palette was generated with Coolors.

## Status

All Lesson 3 tasks are complete: CSS setup, box model mastery, typography
system, and color scheme. All Lesson 4 tasks are complete: Flexbox layout,
CSS Grid layout, mobile-first responsive design, and polish. Everything is
committed and pushed to the `main` branch.

## Author

Built by Alex Morgan — replace with your name and GitHub handle before
committing. This project is part of the IYF S12 web development program,
Week 02.

