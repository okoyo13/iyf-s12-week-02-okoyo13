# IYF S12 · Week 02 · Lesson 3

This repository contains my Lesson 3 work for the IYF S12 program, focused on CSS
foundations. Over the course of four tasks, I moved from a bare HTML page to a
fully styled portfolio with a reusable design system. The work covers base
styling and resets, the CSS box model, a modular typography scale, and a color
scheme built entirely with custom properties. Everything lives in plain HTML
and CSS — no frameworks, no build step, no dependencies.

## Project Structure

The repository is organized into three self-contained pages. At the root,
`index.html` serves as the portfolio homepage and pulls its styles from
`styles.css`, which holds all the design tokens for fonts, the type scale,
colors, and spacing. Inside the `box-model-practice/` folder, you'll find
`index.html` and `styles.css`, which together cover the three box model
exercises — visualizing the model, debugging a width bug, and building a
precisely-spaced card component. Inside `typography-system/`, there's another
`index.html` and `styles.css` pair that showcases the full type scale in a
reference table, so the system can be viewed on its own without the portfolio
content around it. Each folder can be opened directly in a browser.

## What Each Task Covers

Task 3.1 was about setting up a proper stylesheet and establishing base
typography. I linked an external `styles.css` file to every page, applied a
global reset with `margin: 0`, `padding: 0`, and `box-sizing: border-box`, and
defined the root font size at 16px with a line-height of 1.6. Headings from
`h1` through `h6` each get their own size, weight, and consistent bottom
margin, and body text uses a readable slate color instead of pure black.

Task 3.2 lives in the `box-model-practice/` folder and covers the box model
through three exercises. The first shows four boxes side by side, each one
visually breaking down content, padding, border, and margin so the layers are
easy to see. The second takes a broken rule — a 300px box with 20px padding
that renders at 340px — and fixes it by switching from `content-box` to
`border-box`, with both the broken and fixed versions shown side by side for
comparison. The third exercise builds a 300px card with 20px padding, a 1px
solid gray border, a full-width image at the top, a title with exactly 15px of
bottom margin, a short description, and a button at the bottom.

Task 3.3 is the typography system, and it's used both on its own showcase page
and throughout the root portfolio. I paired Montserrat for headings with Open
Sans for body text, then built a modular type scale that runs from 12px at the
small end up to 36px at the largest heading — eight steps in total, stored as
custom properties from `--font-xs` to `--font-4xl`. Each heading level maps to
a specific step: `h1` uses `--font-4xl`, `h2` uses `--font-3xl`, `h3` uses
`--font-2xl`, body text sits at `--font-base`, and small supporting text uses
`--font-sm`.

Task 3.4 adds a color scheme on top of the type system. All colors are defined
as custom properties in `:root`, including a primary brand color, a secondary
accent, light and dark variations of the primary for hover states, plus
background, surface, text, heading, muted, and border colors. These get applied
across headings, body copy, links (with a darker hover state), buttons, and
backgrounds, so every color on the page traces back to a single source of
truth.

## Design Tokens

Every visual decision in this project lives in one `:root` block at the top of
the root `styles.css`. Font families, the eight-step type scale, line heights,
font weights, all the colors, and the spacing scale are all declared there as
custom properties. Because every page imports the same tokens, changing one
value — say, the primary blue — updates the buttons, links, and accents across
the entire site at once. That's the whole point of a token-based system: one
change, one place, everywhere it's needed.

## Getting Started

There's nothing to install. You can either double-click any `index.html` file
and open it in a browser, or — if you'd like the fonts to load consistently
across pages — spin up a simple local server from the project root by running
`python3 -m http.server 8000` in your terminal. Then visit
`http://localhost:8000/` for the portfolio homepage,
`http://localhost:8000/box-model-practice/` for the box model exercises, or
`http://localhost:8000/typography-system/` for the type scale reference.

## Concepts Practiced

The work in this repo touches most of the CSS fundamentals: global resets and
`border-box` sizing, the box model and how padding and borders interact with
width, the difference between `content-box` and `border-box` and when it
matters, card composition with precise spacing, modular type scales, CSS custom
properties as design tokens, font pairing between a heading face and a body
face, and building a color system with light and dark variants for hover
states. Nothing here is framework-dependent — it's all vanilla HTML and CSS.

## References

The MDN Web Docs were my primary reference throughout, especially the *CSS
First Steps* and *The Box Model* pages. For the type scale, I used the online
Type Scale Calculator to generate the eight-step progression from 12px to 36px.
For the color palette, I used Coolors to pick a primary blue and an amber
accent, then derived light and dark variants by hand.

## Status

All four tasks are complete: CSS setup and base styling, box model mastery,
the typography system, and the color scheme. Everything is committed and
pushed to the `main` branch of this repository.

## Author

Built by Alex Morgan — replace this with your name and GitHub handle before
committing. This project is part of the IYF S12 web development program,
Week 02, Lesson 3.

