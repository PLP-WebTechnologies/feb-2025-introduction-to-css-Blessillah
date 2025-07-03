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

Happy Coding! 💻✨
