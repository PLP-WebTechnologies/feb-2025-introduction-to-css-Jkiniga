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

Happy Coding! 💻✨

<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <title>External CSS Example</title>
  <!-- Link to external stylesheet -->
  <link rel="stylesheet" href="style.css">
</head>
<body>

  <!-- Header with an ID selector -->
  <header id="main-header">
    <h1>Welcome to My Styled Page</h1>
  </header>

  <!-- Navigation using a class selector -->
  <nav class="navigation">
    <ul>
      <li><a href="#">Home</a></li>
      <li><a href="#">About</a></li>
      <li><a href="#">Contact</a></li>
    </ul>
  </nav>

  <!-- Main content area -->
  <section class="content">
    <p>
      This is a paragraph demonstrating basic typography, spacing, and colors. Enjoy the styling!
    </p>
    <!-- Image with its own class for styling -->
    <img src="https://via.placeholder.com/400x200"
         alt="Sample Image"
         class="styled-image">
  </section>

  <!-- Footer with another ID selector -->
  <footer id="main-footer">
    <p>&copy; 2025 My Styled Page</p>
  </footer>

</body>
</html>
2. style.css
css
Copy
Edit
/* Import a different font from Google Fonts */
@import url('https://fonts.googleapis.com/css2?family=Roboto:wght@400;700&display=swap');

/* 1. Element selector */
body {
  font-family: 'Roboto', sans-serif;
  line-height: 1.6;
  color: #333;
  margin: 0;
  padding: 0;
  background-color: #f4f4f4;
}

/* 2. ID selector */
#main-header {
  background-color: #4CAF50;
  color: white;
  padding: 20px;              /* Padding */
  text-align: center;
  border-bottom: 4px solid #388E3C;  /* Border */
}

/* 3. Class selector */
.navigation ul {
  list-style: none;
  margin: 0;
  padding: 0;
  display: flex;
  justify-content: center;
  background-color: #fff;
  border-bottom: 1px solid #ccc;
}

.navigation li {
  margin: 0 15px;             /* Margin */
}

.navigation a {
  text-decoration: none;
  color: #4CAF50;
  font-weight: bold;
}

/* Another class selector for the main content */
.content {
  max-width: 800px;
  margin: 20px auto;          /* Center with vertical margin */
  padding: 20px;              /* Padding */
  background-color: #fff;
  border: 2px solid #e0e0e0;  /* Border */
  border-radius: 8px;
}

/* Styling the image */
.styled-image {
  display: block;
  max-width: 100%;
  height: auto;
  margin: 20px auto;          /* Margin around image */
  border: 5px solid #4CAF50;  /* Border */
  border-radius: 10px;        /* Rounded corners */
}

/* Footer styling with ID selector */
#main-footer {
  text-align: center;
  padding: 15px;
  background-color: #333;
  color: #fff;
  margin-top: 20px;
}
