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
/* style.css */

/* --- General Reset & Box Sizing (Good Practice) --- */
* {
    box-sizing: border-box; /* Include padding and border in the element's total width and height */
}

/* --- Body and Root Page Styles (Element Selector) --- */
body {
    font-family: 'Open Sans', sans-serif; /* Different font: A clean, widely used sans-serif font */
    line-height: 1.7; /* Improved readability for text */
    margin: 0; /* Remove default browser margin */
    padding: 30px; /* Overall padding around the content */
    background-color: #e3f2fd; /* A very light blue background */
    color: #3f51b5; /* A shade of indigo for primary text */
}

/* --- Main Content Container (Class Selector) --- */
.container {
    max-width: 1000px; /* Max width for content */
    margin: 40px auto; /* Center the container with top/bottom margin */
    background-color: #ffffff; /* White background for content */
    border: 2px solid #90caf9; /* A light blue border */
    border-radius: 12px; /* Nicely rounded corners */
    box-shadow: 0 8px 25px rgba(0, 0, 0, 0.1); /* Soft, noticeable shadow */
    padding: 30px; /* Internal padding for the container */
}

/* --- Primary Heading Styling (Element Selector) --- */
h1 {
    color: #2196f3; /* A vibrant blue for the main heading */
    text-align: center;
    margin-bottom: 35px; /* Space below the heading */
    padding-bottom: 15px; /* Padding above the bottom border */
    border-bottom: 4px double #bbdefb; /* A double line border below heading */
    font-size: 3em; /* Larger font size */
    text-shadow: 1px 1px 2px rgba(0, 0, 0, 0.05); /* Subtle text shadow */
}

/* --- Secondary Heading Styling (Element Selector) --- */
h2 {
    color: #42a5f5; /* A slightly lighter blue for subheadings */
    margin-top: 40px; /* More space above subheadings */
    margin-bottom: 20px; /* Space below subheadings */
    padding-left: 15px; /* Padding to the left of text */
    border-left: 6px solid #64b5f6; /* Prominent left border accent */
    font-size: 2.2em;
}

/* --- Paragraph Styling (Element Selector) --- */
p {
    margin-bottom: 22px; /* Consistent spacing between paragraphs */
    font-size: 1.15em; /* Slightly larger text for readability */
    color: #455a64; /* A dark grey-blue for body text */
}

/* --- Highlighted Text (Class Selector) --- */
.highlight {
    background-color: #fff9c4; /* Light yellow background for highlight */
    color: #f57f17; /* Dark orange text for highlight */
    font-weight: bold;
    padding: 3px 8px; /* Padding around the highlighted text */
    border-radius: 4px;
}

/* --- Image Styling (Element Selector and ID Selector) --- */
img {
    max-width: 100%; /* Ensures images are responsive */
    height: auto; /* Maintains aspect ratio */
    display: block; /* Makes image a block element, allowing margin: auto for centering */
    margin: 40px auto; /* Generous top/bottom margin, and horizontally centered */
    border: 6px outset #81d4fa; /* An "outset" border for a 3D effect */
    border-radius: 15px; /* More pronounced rounded corners */
    padding: 10px; /* Space between the image content and its border */
    box-shadow: 0 10px 30px rgba(0, 0, 0, 0.2); /* Stronger shadow for depth */
}

/* --- Specific Image Styling (ID Selector) --- */
#gallery-image {
    border-color: #cddc39; /* A lime green border for this specific image */
    border-style: groove; /* A "groove" border style */
    max-width: 75%; /* Make it slightly smaller than other images */
    filter: grayscale(20%); /* Apply a slight grayscale effect */
}

/* --- List Styling (Element Selector) --- */
ul {
    list-style-type: none; /* Remove default bullets */
    padding: 0; /* Remove default padding */
    margin-left: 0;
    margin-bottom: 25px;
}

ul li {
    background-color: #e1f5fe; /* Very light blue background for list items */
    margin-bottom: 12px; /* Space between list items */
    padding: 12px 20px; /* Padding inside list items */
    border: 1px dashed #b3e5fc; /* Dashed border for each list item */
    border-radius: 8px; /* Rounded corners for list items */
    position: relative; /* For custom bullet */
}

/* Custom bullet point for list items */
ul li::before {
    content: '★'; /* Unicode star character */
    color: #ffc107; /* Gold star */
    font-size: 1.2em;
    position: absolute;
    left: 8px; /* Position the star */
    top: 50%;
    transform: translateY(-50%);
}

ul li {
    padding-left: 35px; /* Adjust padding to make space for the custom bullet */
}


/* --- Footer Styling (Element Selector) --- */
footer {
    text-align: center;
    margin-top: 60px; /* More space above the footer */
    padding: 25px; /* Padding inside the footer */
    background-color: #1a237e; /* Dark indigo footer */
    color: #e3f2fd; /* Light blue text for footer */
    font-size: 1em;
    border-top: 3px solid #7986cb; /* Light indigo top border */
    border-radius: 0 0 12px 12px; /* Rounded bottom corners if inside container, or just styled */
}
/* style.css */

/* --- Universal Box Sizing Reset (Best Practice) --- */
* {
    box-sizing: border-box; /* Ensures padding and border are included in an element's total width and height */
}

/* --- Body and Overall Page Styling (Element Selector) --- */
body {
    font-family: 'Lato', sans-serif; /* Different font: A clean and modern sans-serif font */
    line-height: 1.6; /* Improved line spacing for readability */
    margin: 0; /* Remove default browser margin */
    padding: 25px; /* Overall padding around the main content area */
    background-color: #f8f9fa; /* Very light gray background */
    color: #343a40; /* Dark gray text for good contrast */
}

/* --- Header Section Styling (Element Selector) --- */
header {
    background-color: #ffffff; /* White background for header */
    padding: 20px 0; /* Vertical padding */
    margin-bottom: 30px; /* Space below the header */
    border-bottom: 1px solid #e0e0e0; /* Subtle bottom border */
    text-align: center;
    box-shadow: 0 2px 5px rgba(0, 0, 0, 0.05); /* Light shadow */
}

/* --- Main Heading Styling (Element Selector) --- */
h1 {
    color: #007bff; /* Vibrant blue for the main heading */
    font-size: 3.2em; /* Larger font size */
    margin: 0; /* Remove default margin */
    padding: 0; /* Remove default padding */
    letter-spacing: 0.8px;
    text-transform: uppercase;
}

/* --- Subheading Styling (Element Selector) --- */
h2 {
    color: #495057; /* Darker gray for subheadings */
    font-size: 2em; /* Good size for sections */
    margin-top: 40px; /* Space above subheadings */
    margin-bottom: 20px; /* Space below subheadings */
    border-bottom: 2px dashed #ced4da; /* Dashed bottom border */
    padding-bottom: 8px; /* Padding above dashed line */
    text-align: left;
}

/* --- Main Content Wrapper (Class Selector) --- */
.container {
    max-width: 900px; /* Max width for content */
    margin: 0 auto; /* Center the container horizontally */
    background-color: #ffffff; /* White background for content */
    border: 1px solid #dee2e6; /* Light gray border */
    border-radius: 8px; /* Slightly rounded corners */
    box-shadow: 0 5px 15px rgba(0, 0, 0, 0.1); /* Medium shadow for depth */
    padding: 30px; /* Internal padding for the container */
}

/* --- Paragraph Styling (Element Selector) --- */
p {
    margin-bottom: 20px; /* Space between paragraphs */
    font-size: 1.1em; /* Slightly larger text for readability */
}

/* --- Highlighted Text (Class Selector) --- */
.highlight {
    background-color: #fff3cd; /* Light yellow background */
    color: #856404; /* Darker yellow/brown text */
    font-weight: 700; /* Bold text */
    padding: 2px 7px; /* Padding around the highlighted text */
    border-radius: 4px; /* Slightly rounded corners for highlight */
    border: 1px solid #ffeeba; /* Subtle border for highlight */
}

/* --- Image Styling (Element Selector and ID Selector) --- */
img {
    max-width: 100%; /* Ensures images are responsive */
    height: auto; /* Maintains aspect ratio */
    display: block; /* Makes image a block element, allowing margin: auto for centering */
    margin: 30px auto; /* Generous top/bottom margin, and horizontally centered */
    border: 5px solid #28a745; /* Green solid border */
    border-radius: 10px; /* Rounded corners */
    padding: 8px; /* Space between the image content and its border */
    box-shadow: 0 8px 20px rgba(0, 0, 0, 0.1); /* Soft shadow for depth */
}

/* --- Specific Feature Image Styling (ID Selector) --- */
#feature-image {
    border-color: #dc3545; /* Red border for this specific image */
    border-style: ridge; /* Ridge border style */
    max-width: 70%; /* Make it slightly smaller */
    filter: brightness(1.05); /* Slightly brighten the image */
    transition: transform 0.3s ease-in-out; /* Smooth hover effect */
}

#feature-image:hover {
    transform: scale(1.02); /* Slight zoom on hover */
}

/* --- List Styling (Element Selector) --- */
ul {
    list-style-type: none; /* Remove default bullets */
    padding: 0; /* Remove default padding */
    margin-left: 0;
    margin-bottom: 25px;
}

ul li {
    background-color: #e9ecef; /* Light gray background for list items */
    margin-bottom: 10px; /* Space between list items */
    padding: 12px 15px; /* Padding inside list items */
    border-left: 5px solid #007bff; /* Blue left border accent */
    border-radius: 5px; /* Rounded corners for list items */
    font-size: 1.05em;
}

/* --- Footer Styling (Element Selector) --- */
footer {
    text-align: center;
    margin-top: 50px; /* Space above the footer */
    padding: 25px; /* Padding inside the footer */
    background-color: #343a40; /* Dark gray footer background */
    color: #e9ecef; /* Light gray text for footer */
    font-size: 0.95em;
    border-top: 3px solid #6c757d; /* Medium gray top border */
    border-radius: 8px; /* Rounded corners for the footer block */
}
Happy Coding! 💻✨
