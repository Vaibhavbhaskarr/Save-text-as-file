# Save-text-as-file
## A simple program, which saves the text entered as a file 

In this Git Repository you will find 3 files:

    1. index.html: -This file includes the html code for the program. and it links to "style.css" & "script.js".
    2. style.css: -Includes the formating or styling for our program.
    4. script.js: -Includes the functionality of the program.

Further Comments are put inside the code to explain what each part does.

#### HTML 
First we will be taking a look at the HTML part of our program
``` <!DOCTYPE html>
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
