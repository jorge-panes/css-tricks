# Interactive Card Grid Example

This repository showcases a CSS trick for creating an interactive card grid. The cards in the grid adjust their size based on the viewport's width and feature interactive hover effects that highlight the focused card while subtly diminishing the prominence of others.

## Live Version

Explore the interactive card grid in action at [https://jorge-panes.github.io/css-tricks/hover-effect/](https://jorge-panes.github.io/css-tricks/hover-effect/). This live version provides a hands-on demonstration of the card grid's responsiveness and hover effects.

## Project Structure

- `index.html`: The main HTML file contains the layout for the card grid.
- `style.css`: This stylesheet applies the visual and interactive styles to the cards within the grid.

## CSS Trick Highlights

- **Grid Layout**: Utilizes CSS Grid to dynamically arrange cards with `auto-fill` and `minmax` for flexible, responsive layout.
- **Interactive Hover Effects**: Implements a scale transformation on hover for the focused card, while other cards receive a blur effect and scale down, creating a focus on the hovered item.
- **CSS Transitions**: Smooth transitions for scale and blur effects enhance the user interaction experience.

## Viewing the Project

To view this project:
1. Clone this repository to your local machine.
2. Open the `index.html` file in a web browser to see the card grid in action.

Alternatively, visit the live version linked above to see the card grid without downloading or setting up the project locally.

## CSS Code Snippet

Here is a simplified version of the CSS used to achieve the interactive card grid effect:

```css
.cards {
    display: grid;
    grid-template-columns: repeat(auto-fill, minmax(200px, 1fr));
    gap: 20px;
    padding: 20px;
}

.card {
    background: rgb(115, 110, 110);
    display: flex;
    justify-content: center;
    align-items: center;
    border-radius: 8px;
    height: 100px;
    padding: 15px;
    box-shadow: 0 2px 4px rgba(0,0,0,0.2);
    overflow: hidden;
    transition: transform 0.3s ease, box-shadow 0.3s ease;
}

.cards .card:hover {
    transform: scale(1.2);
}

.cards:hover > .card:not(:hover) {
    filter: blur(10px);
    transform: scale(0.9);
}
