# Lychee Facts Explorer

This is a simple webpage that displays interesting facts about lychees. It's designed to be easy to use and provides a visually appealing way to learn about this fruit.

## How to Use

1.  **View the Page:** The `index.html` file contains all the necessary code to display the webpage directly in your browser, as well as on GitHub.
2.  **Explore Facts:** When the page loads, you'll see an initial lychee fact.
3.  **Get New Facts:** Click the "Next Fact" button to see a new random lychee fact.

## Project Structure

This project is built with HTML, CSS, and JavaScript, all contained within the `index.html` file for easy previewing on GitHub. The facts themselves are stored as a JSON object within the javascript code, eliminating the need for a separate `facts.json` file.

*   **`index.html`:** This file contains:
    *   The HTML structure for the webpage.
    *   Embedded CSS styles to handle the layout and visual appearance of the page.
    *   Embedded JavaScript code that handles displaying the initial fact and generating new facts randomly.
    *   A JSON object that contains all of the lychee facts.
*   **`README.md`:** This file, which you are currently reading, provides a general overview of the project, instructions for use, and details about how the project is structured.

## How it Works

*   The webpage dynamically fetches facts from the javascript object within `index.html`
*   The styling uses CSS to make the content visually appealing, using a linear gradient background and blurred fact container.
*   Each time the "Next Fact" button is clicked, the JavaScript updates the displayed fact to a new random fact in the json object.

## How to Preview on GitHub

1.  **Upload Files:** Upload the `index.html` and `README.md` files to your GitHub repository.
2.  **View Preview:** GitHub will automatically render the `README.md` file at the top of the page. Scroll down below it to see the live webpage preview from the `index.html` file.

## Notes

*   This project is intended for a simple display of facts with some basic styling.
*   The styling is done with inline CSS to make the preview easier.
*   All of the facts are contained in the JavaScript, making it a single file application.

Enjoy exploring amazing facts about lychees!
