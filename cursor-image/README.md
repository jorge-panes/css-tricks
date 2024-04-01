# Custom Cursor Example

This project demonstrates how to customize the web page's cursor using CSS, enhancing the user interface by replacing the default cursor with a custom image. 

## Live Version

You can view a live version of this project at [https://jorge-panes.github.io/css-tricks/cursor-image/](https://jorge-panes.github.io/css-tricks/cursor-image/). This live version showcases the custom cursor in action, providing a tangible example of how CSS can be used to personalize cursor design.

## Project Structure

- `index.html`: The main HTML file contains the structure of the web page. 
- `style.css`: This stylesheet applies the custom cursor effect across the entire web page.
- `/assets/cursor.cur`: The custom cursor image used by the `style.css` to change the cursor appearance.

## Viewing the Project

To see the custom cursor effect, clone this repository to your local machine and open the `index.html` file in a web browser. Alternatively, the live version can be viewed directly by visiting the link provided above.

## Custom Cursor CSS Rule

The project uses the following CSS rule to set the webpage's cursor to a custom image (`cursor.cur`) located in the `assets` directory, with a fallback to the browser's default cursor (`auto`) if the custom cursor cannot be loaded:

```css
body {
    cursor: url('../assets/cursor.cur'), auto;
}
