# Debugging Assignment Files

## HTML
- empty meta tag with no attribute, fixed added a charset
  Element meta is missing one or more of the following attributes: charset, content, http-equiv, itemprop, name,
  <meta charset="utf-8">

- img tag in the header was missing alt, fixed added alt txt
  An img element must have an alt attribute, except under certain conditions.
  <img src="./images/easter-bunny-150-profile.png" alt="Easter bunny">

- a p tag was place inside a heading element, closed the h3 before the p tag
  Element p not allowed as child of element h3 in this context.
  <h3>Enough Content</h3>
  <p>You need enough content …</p>


- in the article tag some elements were open, fixed ,corrected the tag order and closed all the tags
  Error: End tag article seen, but there were open elements.
  <article>
  </article>

- multiple br tags, fixed by removing the extra br tags
  <br>

- duplicate @import, fixed by removing and only keeping one instance
  Removed the duplicate Google Fonts @import line.
  @import url('https://fonts.googleapis.com/css2?family=Architects+Daughter&family=Love+Ya+Like+A+Sister&display=swap');
- body tag missing, fixed by adding the closing body tag
 </body>
 </html>

- fixed the hierarchie for the h tags
- updated the assest path for layout.css and image
  <link rel="stylesheet" href="css/layout.css">

## css - style.css/ layout.css
- remove duplicate stylesheet
- corrected the hex colors
  footer    Value Error : color #B2 is not a valid color 3 or 6 hexadecimals numbers : #B2
  footer { color: #B2D732; }
- fixed unit typo errors
  h1    Value Error : font-size Too many values or values are not recognized : 5 vw
  h1 { font-size: 5vw; }
- corrected text decorator
  p Value Error : line-height Unknown dimension 1.35me
  p { line-height: 1.35em; }
- correct the footer color
  .error    Value Error : color #FE27122 is not a valid color 3 or 6 hexadecimals numbers : #FE27122
  footer { background-color: #FE2712; }
- fixed the text-decorator
  a:hover   Value Error : text-decoration all is not a text-decoration value : all
  a:hover { text-decoration: none; }

- fixed nested selectors inside aside
  aside Parse Error dt { font-weight: bold; } dd { padding: 0 10px; }
  aside {
  position: relative;
  padding: 8px 16px;
  margin: 0;
  width: 20vw;
  height: auto;
  float: right;
  }

aside dt { font-weight: bold; }
aside dd { padding: 0 10px; }

- fixed boreder-box
 