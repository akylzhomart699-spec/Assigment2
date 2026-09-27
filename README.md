# Assignment 2 — Advanced CSS

**Jomart Akylbek · IT2507**

Open `index.html` directly in a browser. No installation or server is needed.

Report: [Assignment2_Jomart_Akylbek.docx](Assignment2_Jomart_Akylbek.docx). Open and edit the report in Microsoft Word; screenshots are embedded in the document.

- `index.html` + `composition.css`: seven blocks in a single 6 × 6 Grid, matching the PDF reference.
- `components.html` + `components.css`: five Flexbox components.
- `layouts.html`, `layouts-list.html`, `layouts-magazine.html` + `layouts.css`: twelve identical articles in three layouts.
- `shared.css`: shared colors, typography and spacing.

For Task 3, change only `layout-grid` to `layout-list` or `layout-magazine` on the `.journal` container. The three demonstration files are identical except for this one class. The view links open these static copies so the examples work without JavaScript.

No Bootstrap, JavaScript, media queries, floats or absolute positioning are used in the assignment pages.

## Before submission

The Word report includes screenshots and draft explanations. Review the explanations, rewrite them in your own words, and make sure you can explain the code at the defense. The assignment requires an individual defense and an independent live coding exercise.

Repository: https://github.com/akylzhomart699-spec/Assigment2

When updating the assignment, commit and push the source and updated Word report together.

## Defense notes

- Grid places items along rows and columns. `grid-area` gives start row / start column / end row / end column; end lines are exclusive.
- `aspect-ratio: 1` keeps the composition square; `88vmin` limits it using the smaller viewport dimension.
- The black container shows through `gap`; a matching padding frames the outer edge.
- `flex-wrap` allows navigation and cards to move onto new lines; `margin-inline-start: auto` pushes actions to the right.
- Cards stretch to the same height within each row. Their bodies grow and the button's automatic top margin takes remaining space.
- Pagination uses equal flexible side regions to center the page links, with the count aligned right. Narrow layouts may wrap.
- The comment avatar does not shrink; text lives in a separate flexible child with `min-inline-size: 0` and can wrap long words.
- Pricing uses `align-items: center`; extra content and vertical padding make the recommended plan naturally taller.
- Card Grid uses `auto-fit` and `minmax`; list Grid has one column and Flexbox rows; magazine Grid lets the lead span two columns and two rows.
- A flexible basis such as `flex: 1 1 17rem` is a preferred size, not a fixed width. It may grow or shrink.
