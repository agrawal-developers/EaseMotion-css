# React Search Autocomplete Dropdown with Highlight Motion

A clean React component for autocomplete search with smooth dropdown animations and real-time text highlight matching.

## Features
- highlight text matches
- staggered dropdown fade-in 
- 0 dependencies
- responsive & a11y support

## Installation
Drop `SearchAutocomplete.jsx` and `style.css` into your project.

## Usage

```jsx
import React from 'react';
import SearchAutocomplete from './SearchAutocomplete';

export default function App() {
  const fruits = [
    'Apple', 'Banana', 'Blueberry', 'Cherry', 
    'Grape', 'Mango', 'Orange', 'Strawberry'
  ];

  return (
    <div style={{ padding: '2rem' }}>
      <h2>Search Fruits</h2>
      <SearchAutocomplete 
        items={fruits} 
        placeholder="Type a fruit..." 
        onSelect={(item) => console.log('Selected:', item)}
      />
    </div>
  );
}
```

## Props

| Prop | Type | Description |
|------|------|-------------|
| `items` | Array | Array of strings to filter and display in the dropdown. |
| `placeholder` | String | Placeholder text for the input field. |
| `onSelect` | Function | Callback triggered when a dropdown item is clicked. |
