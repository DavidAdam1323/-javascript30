# Day 2 Challenge: CSS + JS Clock  

## Overview  
Build a real-time analog clock using **HTML, CSS, and JavaScript**. The clock updates every second, with smooth transitions for the hour, minute, and second hands.  

## How it Works  
- The **second, minute, and hour hands** are rotated based on the current system time.  
- `setInterval()` updates the clock every second.  
- CSS transitions make the hands move smoothly.  
- A fixed **middle point** keeps the hands visually centered.  

## Key Concepts Learned  

### DOM Selection  
- Use `document.querySelector` to select the clock hands dynamically.  
- Example:  
  ```js
  const secHand = document.querySelector(".sec-hand");

### Time to Degrees Conversion
- **Seconds** → `(seconds / 60) * 360 + 90`
- **Minutes** → `(minutes / 60) * 360 + (seconds / 60) * 6 + 90`
- **Hours** → `(hours / 12) * 360 + (minutes / 60) * 30 + 90`
- The extra `+90` accounts for the default 90° offset in CSS rotation.

### Smooth Hand Movement
- Minute and hour hands move incrementally based on smaller units:
  - Minutes account for **seconds**  
  - Hours account for **minutes**  
- This creates a natural, continuous motion instead of jumping each tick.

### Flicker-Free Transition
- The second hand resets at `59 → 0`.  
- Without handling, CSS transitions cause a flicker.  
- Conditional logic disables the transition at `0s` to keep it smooth.  

### CSS Centering
- Used `transform: translate(-50%, -50%)` to perfectly center the clock’s middle point.

## Learning Outcomes
- Linking **JavaScript’s Date object** with DOM updates.  
- Using **CSS transforms and transitions** to animate UI elements.  
- Handling **edge cases** (like flickering resets).  
- Writing maintainable, event-driven JavaScript.  
