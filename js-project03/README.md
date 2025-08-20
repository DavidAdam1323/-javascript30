# Day 3 Challenge: CSS Variables & JavaScript

## Overview
Build an interactive web page where users can dynamically update CSS variables using JavaScript, instantly affecting the styling of an image and layout controls.

## How it Works
- Users can adjust **spacing**, **blur**, and **base color** via input controls.
- Changes are applied in real-time using CSS variables.
- The image styling updates dynamically as users interact with the sliders and color picker.

## Key Concepts Learned
### CSS Variables
- CSS custom properties (variables) are defined in `:root` for global usage.
- Example: `--spacing: 10px; --blur: 10px; --base: #ffc600;`
- Variables can be referenced in CSS using `var(--variable-name)`.

### DOM Selection
- `document.querySelectorAll(".controls input")` selects all input elements inside the `.controls` container.
- Each input is tied to a specific CSS variable via its `name` attribute.

### Event Handling
- `input.addEventListener("change", handleUpdate)` triggers updates after input changes.
- `input.addEventListener("mousemove", handleUpdate)` provides real-time feedback as sliders are dragged.

### Dynamic CSS Updates
- `document.documentElement.style.setProperty("--name", value)` dynamically updates a CSS variable.
- For inputs that need units (like `px`), `dataset.sizing` is used to append the correct unit.

### Destructuring
- `const { name, value, dataset } = this;` cleanly extracts relevant input properties for updating CSS variables.

### Responsive Design
- Flexbox layout ensures controls and content adjust for smaller screens.
- Media queries handle column layout for narrow viewports.

## Learning Outcomes
- Dynamically manipulate CSS variables with JavaScript.
- Link form inputs to live style updates on the page.
- Understand and use event-driven programming for interactive UI.
- Apply modern CSS techniques like `var()`, flexbox, and responsive design.
