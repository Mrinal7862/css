# Types of C.S.S.

## Inline C.S.S. 

Css written inside the tags or the element.
```html
    <!-- Inline C.S.S. -->
    <h1 style="background-color: aquamarine; font-family: 'Lucida Sans', 'Lucida Sans Regular', 'Lucida Grande', 'Lucida Sans Unicode', Geneva, Verdana, sans-serif;">
        Hello My name is Mrinal Devnath
    </h1>
```

## Internal C.S.S. 
``` html
<!--Internal C.S.S.-->

    <!DOCTYPE html>
    <html lang="en">
    <head>
        <meta charset="UTF-8">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <title>style1_css</title>

        <style>
                h2{
                    background-color: blueviolet;
                    color:white;
                }
        </style>
    </head>
    <body>
        <!--Internal C.S.S.-->
        <h2>I'm pursuing Computer Science Engineering. </h2>
    </body>
    </html>
```

# External C.S.S.

To use external CSS in your HTML, you'll link the CSS file to your HTML document using the `<link>` tag inside the `<head>` section. This is how you include an external CSS file:

### Basic Structure

1. **HTML File (index.html):**
   ```html
   <!DOCTYPE html>
   <html lang="en">
   <head>
       <meta charset="UTF-8">
       <meta name="viewport" content="width=device-width, initial-scale=1.0">
       <title>My Website</title>
       <!-- Link to the external CSS file -->
       <link rel="stylesheet" href="styles.css">
   </head>
   <body>
       <h1>Welcome to My Website</h1>
       <p>This is a paragraph styled by external CSS.</p>
   </body>
   </html>
   ```

2. **CSS File (styles.css):**
   ```css
   /* External CSS file: styles.css */

   body {
       font-family: Arial, sans-serif;
       background-color: #f0f0f0;
       color: #333;
       margin: 0;
       padding: 0;
   }

   h1 {
       color: #007BFF;
       text-align: center;
       margin-top: 50px;
   }

   p {
       font-size: 18px;
       line-height: 1.6;
       text-align: center;
   }
   ```

### Explanation:

- **HTML File:**
  - The `<link>` tag in the `<head>` section of the HTML file connects the CSS file `styles.css` to the HTML document.
  - The `href` attribute in the `<link>` tag specifies the path to the CSS file.

- **CSS File:**
  - The CSS file contains the styles that are applied to the HTML elements.
  - In this example, the CSS rules set the background color, font family, and text color for the body, as well as the styling for the `<h1>` and `<p>` elements.

### File Organization:
- Keep your HTML and CSS files in the same directory, or adjust the `href` path in the `<link>` tag if the CSS file is located in a different directory.

### Example Directory Structure:
```
/my-website
    /index.html
    /styles.css
```

This method of using external CSS helps in maintaining clean and organized code, especially when working on larger projects where the same styles are applied across multiple HTML files.
