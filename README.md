# Debugging Assignment Files

## HTML

- **Empty meta tag with no attribute** — fixed by adding a `charset`.

Element meta is missing one or more of the following attributes: charset, content, http-equiv, itemprop, name.
 ```html
 <!-- <meta charset="utf-8"> -->
 ```

- **`img` tag in the header was missing alt** — fixed by adding alt text.  
  An img element must have an alt attribute, except under certain conditions.
 ```html
 <!-- <img src="./images/easter-bunny-150-profile.png" alt="Easter bunny"> -->
 ```

- **A `p` tag was placed inside a heading element** — closed the `h3` before the `p` tag.  
  Element `p` not allowed as child of element `h3` in this context.
 ```html
 <!-- <h3>Enough Content</h3> -->
 <!-- <p>You need enough content …</p> -->
 ```

- **In the `article` tag some elements were open** — corrected the tag order and closed all the tags.  
  Error: End tag `article` seen, but there were open elements.
 ```html
 <!-- <article> -->
 <!--   ... -->
 <!-- </article> -->
 ```

- **Multiple `<br>` tags** — fixed by removing the extra `<br>` tags.
 ```html
 <!-- <br> -->
 ```

- **Duplicate `@import`** — fixed by removing and only keeping one instance.  
  Removed the duplicate Google Fonts `@import` line.
 ```css
 /* @import url('https://fonts.googleapis.com/css2?family=Architects+Daughter&family=Love+Ya+Like+A+Sister&display=swap'); */
 ```

- **`body` tag missing** — fixed by adding the closing body tag.
 ```html
 <!-- </body> -->
 <!-- </html> -->
 ```

- **Fixed the hierarchy for the heading (`h`) tags**.

- **Updated the asset path for `layout.css` and image**
 ```html
 <!-- <link rel="stylesheet" href="css/layout.css"> -->
 ```


## CSS — style.css / layout.css

- **Removed duplicate stylesheet**

- **Corrected the hex colors**
 ```css
 /* footer    Value Error : color #B2 is not a valid color 3 or 6 hexadecimals numbers : #B2 */
 /* footer { color: #B2D732; } */
 ```

- **Fixed unit typo errors**
 ```css
 /* h1    Value Error : font-size Too many values or values are not recognized : 5 vw */
 /* h1 { font-size: 5vw; } */

 /* p  Value Error : line-height Unknown dimension 1.35me */
 /* p { line-height: 1.35em; } */
 ```

- **Corrected the footer color**
 ```css
 /* .error    Value Error : color #FE27122 is not a valid color 3 or 6 hexadecimals numbers : #FE27122 */
 /* footer { background-color: #FE2712; } */
 ```

- **Fixed the text-decorator**
 ```css
 /* a:hover   Value Error : text-decoration all is not a text-decoration value : all */
 /* a:hover { text-decoration: none; } */
 ```

- **Fixed nested selectors inside `aside`**
 ```css
 /* aside Parse Error dt { font-weight: bold; } dd { padding: 0 10px; } */

 /* aside {
 /*   position: relative; */
 /*   padding: 8px 16px; */
 /*   margin: 0; */
 /*   width: 20vw; */
 /*   height: auto; */
 /*   float: right; */
 /* } */

 /* aside dt { font-weight: bold; } */
 /* aside dd { padding: 0 10px; } */
 ```

- **Fixed border-box**
 ```css
 /* *, *::before, *::after {
 /*   box-sizing: border-box;
 /* } */
 ```