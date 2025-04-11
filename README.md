# Modern CSS Slider

![Modern CSS Slider](https://picsum.photos/id/10/800/200)

## 📋 Overview

This project is a modern, responsive card slider created with pure CSS. It features beautiful cards with images, badges, and interactive elements. The slider works on all devices and has smooth animations.

## ✨ Features

- 🎨 Modern design with gradient colors
- 📱 Fully responsive (works on mobile, tablet, and desktop)
- 🔄 Smooth sliding animations
- 💫 Interactive hover effects
- 🏷️ Card badges and tags
- 🖱️ Scroll buttons and markers
- ✨ Shine effect on hover

## 🚀 How to Use

1. Clone this repository
2. Open `index.html` in your browser
3. Enjoy the slider!

## 🔧 How It Works

### HTML Structure

The slider is built with a simple HTML structure:

```html
<div class="carousel-container">
    <ul class="carousel">
        <li>
            <div class="card">
                <!-- Card content here -->
            </div>
        </li>
        <!-- More cards here -->
    </ul>
</div>
```

Each card has:
- Image section with badge
- Content section with title and description
- Footer with tag and button

### CSS Features Explained

#### 1. Variables

The project uses CSS variables for colors, shadows, and transitions:

```css
:root {
  --primary-color: #4361ee;
  --secondary-color: #3a0ca3;
  --accent-color: #f72585;
  /* More variables... */
}
```

You can easily change the colors by editing these variables.

#### 2. Carousel System

The carousel uses modern CSS Grid for layout:

```css
.carousel {
  display: grid;
  grid-auto-flow: column;
  grid-auto-columns: 40%;
  gap: 2rem;
  /* More properties... */
}
```

It also uses `scroll-snap` to create a smooth snapping effect when scrolling.

#### 3. Card Design

Cards have several interactive effects:
- 3D rotation on hover
- Image scale and brightness change
- Shine animation effect
- Shadow changes

#### 4. Scroll Controls

The slider has built-in scroll buttons and markers:

```css
.carousel::scroll-button(left),
.carousel::scroll-button(right) {
  /* Button styles */
}

.carousel li::scroll-marker {
  /* Marker styles */
}
```

#### 5. Responsive Design

The slider adapts to different screen sizes:

```css
@media (max-width: 768px) {
  .carousel {
    grid-auto-columns: 100%;
    /* More mobile styles... */
  }
}
```

## 📝 How to Add More Cards

To add more cards to the slider, follow these steps:

1. Open `index.html`
2. Copy an existing `<li>` element with its card
3. Paste it inside the `<ul class="carousel">` element
4. Change the content:
   - Update the image URL
   - Change the badge text
   - Edit the title and description
   - Update the tag name

Example of a new card:

```html
<li>
    <div class="card">
        <div class="card-image">
            <img src="https://picsum.photos/id/15/800/450" alt="New Image">
            <div class="card-badge">New Badge</div>
        </div>
        <div class="card-content">
            <h3>New Title</h3>
            <p>New description text goes here.</p>
            <div class="card-footer">
                <span class="card-tag">New Tag</span>
                <button class="card-button">View More</button>
            </div>
        </div>
    </div>
</li>
```

## 🎨 How to Customize

### Change Colors

Edit the CSS variables in `styles.css`:

```css
:root {
  --primary-color: #YOUR_COLOR;
  --secondary-color: #YOUR_COLOR;
  --accent-color: #YOUR_COLOR;
  /* More variables... */
}
```

### Change Card Size

Modify the grid column size:

```css
.carousel {
  grid-auto-columns: 40%; /* Change this value */
}
```

### Change Animation Speed

Edit the transition variable:

```css
:root {
  --transition: all 0.3s cubic-bezier(0.25, 0.8, 0.25, 1); /* Change timing */
}
```

## 📱 Browser Support

This slider works in all modern browsers:
- Chrome
- Firefox
- Safari
- Edge

Some advanced features might not work in older browsers.

## 🤝 Contributing

Feel free to fork this project and add your own features!

## 📄 License

This project is open source and available under the MIT License.
