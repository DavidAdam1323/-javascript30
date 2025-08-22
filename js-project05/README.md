# Day 5 Challenge: Flex Panel Image Gallery

## Overview
Working on interactive image gallery using CSS Flexbox where panels expand with smooth animations when clicked, revealing additional text content with elegant transitions.

## How it Works
- Click on any panel to expand it while others contract
- Expanded panel grows to 5x its original size with smooth animation
- Text elements slide in from top and bottom when panel is active
- Transitionend event triggers secondary animation for text elements

## Key Concepts Learned
### CSS Flexbox Layout
- Use `display: flex` to create flexible container layouts
- `flex: 1` distributes space equally among panels initially
- `flex: 5` expands the active panel to take more space

### CSS Transitions and Animations
- Implement smooth transitions with `transition` property
- Use custom timing functions with `cubic-bezier()` for natural motion
- Coordinate multiple transitions (font-size, flex, background)

### CSS Background Properties
- Set responsive background images with `background-image`
- Use `background-size: cover` and `background-position: center` for optimal image display

### JavaScript Event Handling
- `querySelectorAll()` to select multiple elements
- `addEventListener("click", toggleOpen)` for panel interaction
- `addEventListener("transitionend", toggleActive)` for animation sequencing

### Class Manipulation
- `classList.toggle()` to add/remove classes dynamically
- Use CSS classes to control visual states (open, open-active)

### Transform Properties
- `transform: translateY(-100%)` and `transform: translateY(100%)` to position text off-screen
- Animate text elements into view with transform transitions

### Event Property Detection
- `e.propertyName.includes("flex")` to identify specific transition events
- Ensure actions trigger only after the correct animation completes

## Learning Outcomes
- Creating responsive layouts with CSS Flexbox
- Implementing complex CSS transitions and animations
- Coordinating multiple animated elements with JavaScript
- Building interactive image galleries with smooth user experience
- Using event listeners to create sequenced animations
- Mastering class-based state management for UI components