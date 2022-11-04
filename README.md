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
In the first part of our CSS code, we import the font that we would like to use, then we use `*` to assign the following styles to all the elements, the font, margin, padding and box-sizing. 

Then for the `body`, we align the items in the `center` and justify the content to `center`. The padding and background color are set. For display we use `flex` so that the child elements can be auto assigned aligned flexibly. 

```CSS
.wrapper{
  width: 443px;
  border-radius: 7px;
  background: #fff;
  padding: 30px 25px 40px;
  box-shadow: 0 10px 15px rgba(0,0,0,0.05);
}
.wrapper :where(textarea, input, select, button){
  width: 100%;
  outline: none;
  border: none;
  font-size: 17px;
  border-radius: 5px;
}
.wrapper :where(textarea, input)::placeholder{
  color: #aaa;
}
.wrapper :where(textarea, input):focus{
  box-shadow: 0px 2px 4px rgba(0,0,0,0.08);
}
.wrapper textarea{
  height: 270px;
  resize: none;
  padding: 8px 13px;
  font-size: 17.6px;
  border: 1px solid #ccc;
}
.wrapper .file-options{
  display: flex;
  margin-top: 10px;
  align-items: center;
  justify-content: space-between;
}

```
In this part of our CSS, we style the `.wrapper` class, adding some padding, box-shadow, width for our box, and also border-radius to add a nice rounding effect to it. In 
```CSS 
.wrapper :where(textarea, input, select, button){ 
``` 
We make changes to the elemnts inside our `.wrapper` class, but these changes would be made **only** to `textarea,input,select,button` elements. A border-radius is added for the rounding effect on the edges. Outline and border are set to 0, and the font-size is set to 17px. Similarly we make further changes to different elements  inside our `.wrapper` class based on our preference. The `.wrapper textarea` is set to `height: 270px`, this determines the height of our textarea.
