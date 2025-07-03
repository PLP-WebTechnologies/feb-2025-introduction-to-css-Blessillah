# Introduction to CSS

## Objectives
Link an external CSS file to an HTML document.
Apply basic styling using selectors.
Use colors, fonts, and spacing effectively.

## Instructions

Create a style.css file.
Apply CSS to a HTML page.
Style elements using:
Classes and IDs.
Color and typography.
Margins, paddings, and borders.

>[!NOTE]
>  - Include at least:
>  - Use of 3 selectors
>  - Style an image
>  - Margin, Padding & Borders
>  - Different font

# Tasks
 - Link an external CSS file.
 - Apply at least 3 different selectors.
 - Improve readability and aesthetics.
   <!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Styled HTML Page</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <div class="container">
        <h1>Welcome to My Styled Page</h1>

        <p>This is a demonstration of applying <span class="highlight">CSS styling</span> to an HTML page. We are using various selectors to make the page more readable and aesthetically pleasing.</p>

        <img src="https://via.placeholder.com/600x300?text=Placeholder+Image" alt="A generic placeholder image for demonstration purposes.">

        <p>Here's another paragraph to show how global paragraph styles work. Notice the font, line height, and margins applied from our `style.css` file.</p>

        <img id="profile-pic" src="https://via.placeholder.com/200x200?text=Profile+Pic" alt="A placeholder for a profile picture.">

        <h2>Key Features Demonstrated:</h2>
        <ul>
            <li>Linking an external CSS file for better organization.</li>
            <li>Applying at least 3 different selectors (element, class, ID).</li>
            <li>Styling an image with borders, padding, and margins.</li>
            <li>Using different font styles and colors for improved aesthetics.</li>
            <li>Implementing margins, padding, and borders on various elements.</li>
        </ul>

        <p class="highlight">This text uses a class selector to apply specific styling, like a different color and bold font.</p>

    </div>

    <footer>
        <p>&copy; 2025 Styled Page Demo. All rights reserved.</p>
    </footer>
</body>
</html>
/* style.css */

/* --- Body and General Styles (Element Selector) --- */
body {
    font-family: 'Verdana', sans-serif; /* Different font */
    line-height: 1.7;
    margin: 25px; /* Margin for the body */
    background-color: #e8f5e9; /* Light green background */
    color: #212121; /* Dark text for readability */
    box-sizing: border-box; /* Include padding and border in the element's total width and height */
}

/* --- Main Content Wrapper (Class Selector) --- */
.wrapper {
    max-width: 900px;
    margin: 30px auto; /* Center the wrapper with top/bottom margin */
    padding: 25px;
    background-color: #ffffff;
    border: 1px solid #c8e6c9; /* Subtle border */
    border-radius: 10px;
    box-shadow: 0 4px 15px rgba(0, 0, 0, 0.08); /* Soft shadow */
}

/* --- Heading Styles (Element Selector) --- */
h1 {
    color: #2e7d32; /* Dark green for headings */
    text-align: center;
    margin-bottom: 25px;
    padding-bottom: 10px;
    border-bottom: 2px dashed #a5d6a7; /* Dashed border for aesthetics */
    font-size: 2.5em;
}

h2 {
    color: #43a047; /* Slightly lighter green for subheadings */
    margin-top: 30px;
    margin-bottom: 15px;
    border-left: 5px solid #81c784; /* Left border for emphasis */
    padding-left: 10px;
}

/* --- Paragraph Styles (Element Selector) --- */
p {
    margin-bottom: 20px; /* Space between paragraphs */
    font-size: 1.05em;
}

/* --- Emphasized Text (Class Selector) --- */
.emphasis-text {
    color: #d32f2f; /* Red color for emphasis */
    font-weight: bold;
    background-color: #ffe0b2; /* Light orange background */
    padding: 2px 5px;
    border-radius: 3px;
}

/* --- Image Styling (Element Selector and ID Selector) --- */
img {
    max-width: 100%; /* Ensures responsiveness */
    height: auto; /* Maintains aspect ratio */
    display: block; /* Centers block elements */
    margin: 25px auto; /* Margin top/bottom and auto for centering */
    border: 5px double #66bb6a; /* Double border */
    padding: 8px; /* Padding inside the border */
    border-radius: 12px; /* Slightly rounded corners */
    box-shadow: 0 6px 12px rgba(0, 0, 0, 0.15); /* More pronounced shadow */
}

/* --- Specific Image Styling (ID Selector) --- */
#hero-image {
    border-color: #1b5e20; /* Darker green border for the hero image */
    border-style: solid; /* Solid border for this specific image */
    max-width: 80%; /* Make it a bit smaller than 100% of its parent */
    margin-bottom: 40px; /* More space below */
}

/* --- List Styles (Element Selector) --- */
ul {
    list-style-type: square; /* Square bullets */
    margin-left: 25px;
    margin-bottom: 20px;
}

ul li {
    background-color: #f1f8e9; /* Very light green background for list items */
    margin-bottom: 10px;
    padding: 10px 15px;
    border-left: 4px solid #66bb6a; /* Left border for list items */
    border-radius: 5px;
}

/* --- Footer Styles (Element Selector) --- */
footer {
    text-align: center;
    margin-top: 50px;
    padding: 20px;
    background-color: #388e3c; /* Dark green footer */
    color: #e8f5e9; /* Light text for footer */
    font-size: 0.9em;
    border-top: 1px solid #2e7d32;
    border-radius: 0 0 10px 10px; /* Rounded bottom corners */
}
/* style.css */

/* --- Universal Box Sizing (Good Practice) --- */
* {
    box-sizing: border-box; /* Ensures padding and border are included in element's total width/height */
}

/* --- Body and General Page Styling (Element Selector) --- */
body {
    font-family: 'Roboto', sans-serif; /* Different font for the whole page */
    line-height: 1.6;
    margin: 0; /* Remove default body margin */
    padding: 20px; /* Overall page padding */
    background-color: #f0f2f5; /* Light grey background */
    color: #333; /* Dark grey text */
}

/* --- Container for Main Content (Class Selector) --- */
.main-container {
    max-width: 960px;
    margin: 30px auto; /* Center the container with top/bottom margin */
    background-color: #ffffff;
    border: 1px solid #ddd; /* Subtle border */
    border-radius: 8px;
    box-shadow: 0 2px 10px rgba(0, 0, 0, 0.08); /* Soft shadow */
    padding: 25px; /* Padding inside the container */
}

/* --- Header Styling (Element Selector) --- */
h1 {
    color: #1a73e8; /* Blue heading color */
    text-align: center;
    margin-bottom: 25px;
    padding-bottom: 10px;
    border-bottom: 3px solid #1a73e8; /* Blue bottom border */
    font-size: 2.8em;
    letter-spacing: 0.5px;
}

/* --- Sub-heading Styling (Element Selector) --- */
h2 {
    color: #3f51b5; /* Slightly darker blue */
    margin-top: 35px;
    margin-bottom: 15px;
    padding-left: 10px;
    border-left: 4px solid #4285f4; /* Left border accent */
    font-size: 1.8em;
}

/* --- Paragraph Styling (Element Selector) --- */
p {
    margin-bottom: 18px; /* Space between paragraphs */
    font-size: 1.1em;
}

/* --- Callout Text (Class Selector) --- */
.callout {
    background-color: #e8f0fe; /* Light blue background */
    border-left: 5px solid #4285f4; /* Blue left border */
    padding: 15px 20px;
    margin: 20px 0;
    font-style: italic;
    color: #0056b3;
    border-radius: 4px;
}

/* --- Image Styling (Element Selector and ID Selector) --- */
img {
    max-width: 100%; /* Make images responsive */
    height: auto; /* Maintain aspect ratio */
    display: block; /* Remove extra space below images and allow margin: auto */
    margin: 30px auto; /* Center images with top/bottom margin */
    border: 4px solid #4CAF50; /* Green border */
    border-radius: 10px; /* Slightly rounded corners */
    padding: 7px; /* Space between image content and border */
    box-shadow: 0 4px 15px rgba(0, 0, 0, 0.15); /* Soft shadow */
}

/* --- Specific Hero Image Styling (ID Selector) --- */
#hero-banner {
    border-color: #ff9800; /* Orange border for this specific image */
    border-width: 6px; /* Thicker border */
    border-style: outset; /* Outset border style */
    margin-bottom: 40px; /* More space below */
    border-radius: 15px;
}

/* --- List Styling (Element Selector) --- */
ul {
    list-style-type: disc; /* Default disc bullets */
    margin-left: 25px;
    margin-bottom: 20px;
}

ul li {
    background-color: #f7f9fc; /* Very light background for list items */
    margin-bottom: 10px;
    padding: 10px 15px;
    border-bottom: 1px dashed #c5cae9; /* Dashed bottom border */
    border-radius: 3px;
    font-size: 1em;
}

/* --- Footer Styling (Element Selector) --- */
footer {
    text-align: center;
    margin-top: 50px;
    padding: 20px;
    background-color: #212121; /* Dark footer background */
    color: #e0e0e0; /* Light grey text */
    font-size: 0.9em;
    border-top: 2px solid #555;
    border-radius: 0 0 8px 8px; /* Rounded bottom corners if used in a container */
}

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Stylish Web Page Example</title>
    <link rel="stylesheet" href="style.css">
    <link href="https://fonts.googleapis.com/css2?family=Roboto:wght@400;700&display=swap" rel="stylesheet">
</head>
<body>
    <div class="main-container">
        <h1>Welcome to Our Beautiful Page</h1>

        <img id="hero-banner" src="https://via.placeholder.com/900x450/4285F4/FFFFFF?text=Stunning+Header+Image" alt="A beautiful placeholder image for the page header.">

        <p>This page is designed to showcase the power of CSS in creating visually appealing and readable web content. We've utilized various styling techniques to make the experience pleasant for the user.</p>

        <div class="callout">
            <p><strong>Did you know?</strong> Effective use of margins, padding, and borders can significantly improve the perceived quality and structure of your web layouts.</p>
        </div>

        <h2>Key Design Elements</h2>
        <p>Here are some of the CSS features demonstrated on this page:</p>
        <ul>
            <li>
                **External CSS Link:** The stylesheet is linked from an external file (`style.css`) for better organization.
            </li>
            <li>
                **Multiple Selectors:** We use element selectors (e.g., `body`, `h1`, `p`), class selectors (e.g., `.main-container`, `.callout`), and ID selectors (e.g., `#hero-banner`).
            </li>
            <li>
                **Responsive Image Styling:** Images adapt to screen size while maintaining their aspect ratio.
            </li>
            <li>
                **Custom Fonts & Colors:** A 'Roboto' font is used, along with a carefully chosen color palette for headings, text, and backgrounds.
            </li>
            <li>
                **Box Model Properties:** Extensive application of `margin`, `padding`, and `border` to control spacing and visual separation.
            </li>
        </ul>

        <h2>Image Responsiveness Explained</h2>
        <img src="https://via.placeholder.com/600x300/F4B400/FFFFFF?text=Responsive+Image+Example" alt="An example of a responsive image adapting to different screen sizes.">
        <p>The image above is set to be responsive using `max-width: 100%;` and `height: auto;`. This ensures it scales down gracefully on smaller screens and doesn't exceed its natural size on larger ones, preventing horizontal scrollbars and maintaining aspect ratio.</p>

    </div>

    <footer>
        <p>Created with CSS Magic &copy; 2025. All rights reserved.</p>
    </footer>
</body>
</html>
Happy Coding! 💻✨
