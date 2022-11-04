# Save-text-as-file
## A simple program, which saves the text entered as a file 

In this Git Repository you will find 3 files:

    1. index.html: -This file includes the html code for the program. and it links to "style.css" & "script.js".
    2. style.css: -Includes the formating or styling for our program.
    4. script.js: -Includes the functionality of the program.

Further Comments are put inside the code to explain what each part does.

#### HTML - First we will be taking a look at the HTML part of our program
```HTML
<!DOCTYPE html>
<html lang="en" dir="ltr">
  <head>
    <meta charset="utf-8">
    <title>Save Text As File | Vaibhav Bhaskar</title>
    <link rel="stylesheet" href="style.css">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <script src="script.js" defer></script>
  </head>
  <body>
    <div class="wrapper">
      <textarea spellcheck="false" placeholder="Enter something to save" required>Hello Programmmerzzzz</textarea>
      <div class="file-options">
        <div class="option file-name">
          <label>File name</label>
          <input type="text" spellcheck="false" placeholder="Enter file name">
        </div>
        <div class="option save-as">
          <label>Save as</label>
          <div class="select-menu">
            <select>
              <option value="text/plain">Text File (.txt)</option>
              <option value="text/javascript">JS File (.js)</option>
              <option value="text/html">HTML File (.html)</option>
              <option value="image/svg+xml">SVG File (.svg)</option>
              <option value="application/msword">Doc File (.doc)</option>
              <option value="application/vnd.ms-powerpoint">PPT File (.ppt)</option>
            </select>
          </div>
        </div>
      </div>
      <button class="save-btn" type="button">Save As Text File</button>
    </div>
    
  </body>
</html> 
```

In the HTML file, the script.js and the style.css files are linked. After which we have added the main components of our code. We have a `textarea` which has a `placeholder` "Enter something to save". There is a dummy default text "Hello Programmmerzzzzz". Then there is another textfield which is for the "Enter file name".  Then comes the `Save as` option, where we use `Select` tag for our drop down menu. 

For the `option` we select the **MIME value** which is the identifier which indicates the nature and format of the document. 

- The MIME value for a text file (txt) is *text/plain*. 
- The MIME value for a javascript file (.js) is *text/javascript*.
- The MIME value for a html file (.html) is *text/html*.
- The MIME value for SVF file (.svg) is *image/svg+xml*.
- The MIME value for a Doc file (.doc) is *application/msword*.
- The MIME value for a PPT file (.ppt) is *application/vnd.ms-powerpoint*.

Lastly a button is added, which will be used as the `Save as text file` button.



#### Next we move on to the CSS part of our program, in which we will be styling our HTML components.

```CSS
@import url('https://fonts.googleapis.com/css2?family=Poppins:wght@400;500;600&display=swap');
*{
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  font-family: 'Poppins', sans-serif;
}
body{
  display: flex;
  align-items: center;
  justify-content: center;
  min-height: 100vh;
  padding: 10px;
  background: #17A2B8;
}
```
