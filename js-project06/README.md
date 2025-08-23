# Day 6 Challenge: Ajax Type Ahead

## Overview
Build a real-time city search interface that filters UK cities as you type, fetching data from a public API and displaying matching results instantly.

## How it Works
- Type in the search input to filter through UK cities in real-time
- Data is fetched from a geonames API containing 500 UK cities
- Matching cities are displayed instantly as you type
- Each result shows the city name and its population

## Key Concepts Learned
### API Data Fetching
- Use `fetch()` to retrieve data from external APIs
- Handle promises with `.then()` to process JSON responses
- Extract and store relevant data in an array for later use

### Regular Expressions for Searching
- Create case-insensitive regex patterns with `new RegExp(wordToMatch, "i")`
- Use `String.match()` to find pattern matches in city names

### Array Filtering
- Filter large datasets based on user input
- Return only matching items with `array.filter()`

### Real-time Input Handling
- Listen for `input` events on search fields
- Trigger filtering and display updates on each keystroke

### Dynamic HTML Generation
- Use `array.map()` to transform data into HTML elements
- Join array elements into a single string with `array.join()`

### Population Formatting
- Format large numbers with `toLocaleString()` for better readability
- Handle potential missing data with fallback values ("N/A")

### Responsive Grid Layout
- Create adaptive layouts with CSS Grid (`grid-template-columns: repeat(auto-fit, minmax(...))`)
- Style cards with hover effects and transitions for better UX

## Learning Outcomes
- Fetching and processing data from external APIs
- Implementing real-time search functionality
- Using regular expressions for pattern matching
- Creating responsive, user-friendly interfaces
- Handling asynchronous data operations in JavaScript
- Generating dynamic content based on user input
- Formatting data for better presentation