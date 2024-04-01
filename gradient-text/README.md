# Text Gradient Trick

This project demonstrates a simple but visually striking text gradient effect using HTML and CSS. It showcases how to apply a linear gradient to text for a colorful and dynamic appearance.

## Live Version

You can view a live version of this project at the following URL: [https://jorge-panes.github.io/css-tricks/gradient-text/](https://jorge-panes.github.io/css-tricks/gradient-text/). This live version is hosted on GitHub Pages, providing an easy way to see the text gradient effect in action.

## Project Structure

- `index.html`: The main HTML file that includes the basic structure of the web page. It contains a `<div>` with a class of `.container` that wraps around a `<h1>` element displaying the text with the gradient effect.
- `style.css`: The stylesheet for the web page. It defines the gradient effect applied to the `<h1>` element text, creating a transition from blue to red.

## Viewing the Project

To view this project, simply clone this repository to your local machine and open the `index.html` file in your preferred web browser. The text gradient effect will be visible on the header text. Alternatively, you can visit the live version linked above.

## CSS for Text Gradient

The key to this effect is the CSS styling applied to the `<h1>` element. Here's a quick look at the CSS used:

```css
h1 {
    background: linear-gradient(90deg, blue, red);
    -webkit-background-clip: text;
    background-clip: text;
    -webkit-text-fill-color: transparent;
}