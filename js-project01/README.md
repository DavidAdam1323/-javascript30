# Day 1 Challenge: JavaScript Drum Kit

## Overview
Build an interactive web page where pressing certain keyboard keys plays drum sounds and visually animates the corresponding buttons.

## How it Works
- Press a key (A, S, D, F, G, H, J, K, L) to play a sound.
- The corresponding button visually animates when pressed.
- Animation resets automatically after the transition ends.

## Key Concepts Learned
### DOM Selection
- Use `document.querySelector` and `document.querySelectorAll` to select HTML elements dynamically.
- Example: `document.querySelector('.key[data-key="A"]')` selects the button for key "A".

### Event Handling
- `window.addEventListener("keydown", playSound)` listens for key presses.
- `key.addEventListener("transitionend", removeTransition)` resets the animation after the transition ends.

### Audio Playback
- `<audio>` elements are linked to keys via `data-key`.
- `audio.play()` triggers sound playback.
- `audio.currentTime = 0` ensures the sound restarts immediately on repeated presses.

### CSS Transitions
- `.key.active` class adds scale and border effects on key press.
- Removed after the transition ends.

### Case-Insensitive Key Matching
- `e.key.toUpperCase()` allows both lowercase and uppercase key presses to trigger the correct sound.

### Graceful Error Handling
- `if (!audio) return;` prevents errors if an unmapped key is pressed.

## Learning Outcomes
- Linking keyboard input to DOM updates.
- Playing audio dynamically with JavaScript.
- Using CSS transitions for interactive feedback.
- Writing event-driven, clean JavaScript code.