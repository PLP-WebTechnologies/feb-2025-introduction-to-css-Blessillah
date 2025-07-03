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

Happy Coding! 💻✨
