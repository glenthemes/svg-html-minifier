![SVG HTML Minifier: one icon? One line. Written by glenthemes](https://user-images.githubusercontent.com/45606634/210125945-402f992e-e086-4788-a434-72c1c43ff4a6.png)

Ever wanted to add an SVG (shape, icon, etc) to your site in HTML but the code is super long and you get lost in your code? [**SVG HTML Minifier**](https://jsfiddle.net/glenthemes/mod5vw48/show) (JS) is a tool that helps you add SVG icons & shapes to your site without including its full SVG code in the HTML! It moves the bulk of the SVG code to JavaScript, so you only need one line of `div` to get the job done. So whilst the code isn't entirely "omitted", it minifies your HTML and makes it easier to scroll through without getting lost between SVGs.

This tool takes the original SVG path and encodes it into a [Data URI format](https://css-tricks.com/data-uris). It becomes a string that can be applied as the [mask](https://css-tricks.com/almanac/properties/m/mask-image) of a div, so the div takes on the shape of the SVG. We can change the SVG's color via the `background-color` CSS property.

---

### <sub>FEATURES:</sub>

* easily set the size and color of SVGs in CSS
* you can use the same SVG multiple times without duplicating the entire SVG code
* if you find a SVG icon library that you like but only want to use a couple icons from it, you can use this method to only load the ones you need
pure JavaScript, no jQuery needed
* I’ve also included instructions on how to minify the JS codes even further if you have multiple complex SVGs!

---

### <sub>LIMITATIONS:</sub>

* only works with SVGs of single color.  
  it will not work with multi-colored SVGs.
* the aggregate SVG codes will get very long in JavaScript. You may consider saving them as a `.js` file and add it to your site as a script.
* since it's not an icon font, you cannot change the line weight/thickness of the SVG.

---

### <sub>DEMO:</sub>

[jsfiddle.net/glenthemes/mod5vw48/show](https://jsfiddle.net/glenthemes/mod5vw48/show)  

![image](https://user-images.githubusercontent.com/45606634/210126225-ead7f909-c699-43e0-82f4-10a6469608ea.png)


Using a [basic circle](https://www.flaticon.com/free-icon/dry-clean_481078) as an example, the SVG code is as follows:
```
<svg xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" version="1.1" id="Layer_1" x="0px" y="0px" viewBox="0 0 512 512" style="enable-background:new 0 0 512 512;" xml:space="preserve">
<g>
<path d="M256,0C115.03,0,0,115.05,0,256c0,140.97,115.05,256,256,256c140.97,0,256-115.05,256-256C512,115.03,396.95,0,256,0z M256,482C131.383,482,30,380.617,30,256S131.383,30,256,30s226,101.383,226,226S380.617,482,256,482z"/>
</g>
</svg>
```

We then give it a name, let's just say `circle`.

Determine how big you want your SVG to be. Let's say `69px`.

Choose a color for your SVG. I've chosen a `#637dff` with RGB values `114, 113, 218`.

Fill that in:  
![image](https://user-images.githubusercontent.com/45606634/210126272-75a57504-9c88-48de-a077-80e4d9724920.png)

Press `Generate` and let the magic happen! The generator will give you the required HTML, CSS, and JavaScript codes, and a preview of what the result looks like:

![image](https://user-images.githubusercontent.com/45606634/210126327-d64cc3d1-688f-472e-8197-3c2451c12d29.png)  
![image](https://user-images.githubusercontent.com/45606634/210126287-d9f71517-f8cf-4191-bfdd-d0a63d6559c5.png)

---

### <sub>MORE INFO:</sub>

[glenthemes.tumblr.com/svg-html-minifier](https://glenthemes.tumblr.com/svg-html-minifier)
