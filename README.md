# Responsive Video Gallery

## Overview

This project is a responsive video gallery layout created with HTML and CSS. The layout features a navigation bar, a section to display videos, and a footer. It is designed to be responsive and looks good on both desktop and mobile devices.

## Features

- **Responsive Design:** Adapts to various screen sizes using CSS media queries.
- **Hover Effects:** Smooth scaling effect on video items when hovered.
- **Navigation Bar:** Simple and centered navigation bar with hover effects.
- **SEO and Accessibility:** Basic SEO meta tags and ARIA landmarks for better accessibility.

## File Structure

- **index.html:** The main HTML file containing the structure of the webpage.
- **main.css:** The CSS file containing styles for the webpage.

### HTML Structure

The HTML file includes:

- A navigation bar with links.
- A section for featured videos with a title.
- Video items within a flexible container.
- A footer for additional information.

### CSS Details

- Global Styles

```bash
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

body {
    font-family: Arial, sans-serif;
    background-color: #f4f4f4;
    color: #333;
}
```

- Navigation Bar

```bash
nav {
    background-color: #333;
    padding: 10px 0;
}

.navbar {
    display: flex;
    justify-content: center;
    list-style: none;
}

.navbar a {
    color: white;
    padding: 14px 20px;
    text-decoration: none;
    text-align: center;
}

.navbar a:hover {
    background-color: #575757;
    transition: background-color 0.3s;
}
```

- Video Container and Items

```bash
.section-title {
    text-align: center;
    margin: 20px 0;
    font-size: 2em;
}

.video-container {
    display: flex;
    flex-wrap: wrap;
    justify-content: space-around;
    padding: 20px;
}

.video-item {
    flex: 1 1 300px; /* Flex-grow, flex-shrink, flex-basis */
    margin: 10px;
    max-width: 350px;
    box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
    background-color: white;
    border-radius: 8px;
    overflow: hidden;
    transition: transform 0.5s ease-in-out;
}

.video-item:hover {
    transform: scale(1.05);
}

.video-item video {
    width: 100%;
    height: auto;
    border: none;
}

.video-description {
    padding: 10px;
    text-align: center;
    font-size: 1em;
}
```

- Footer

```bash
footer {
    background-color: #333;
    color: white;
    text-align: center;
    padding: 10px 0;
}
```

- Responsive Design

```bash
@media (max-width: 768px) {
    .navbar {
        flex-direction: column;
    }

    .video-container {
        flex-direction: column;
        align-items: center;
    }

    .video-item {
        flex: 1 1 100%;
        max-width: 90%;
    }
}
```

## Usage

1. Clone the repository:
```bash
git clone https://github.com/H3nryK/video-gallery.git
```
2. Navigate to the project directory:
```bash
cd video-gallery
```
3. Open `index.html` in your browser to view the responsive video gallery.

## Future Improvements

- Add more interactive features like a "back to top" button.
- Implement lazy loading for videos to improve performance.
- Enhance the design with more CSS animations and transitions.
- Add JavaScript for additional functionality such as video modals.