# CSS
`Inline` css is written in the body and `Internal` style-element inside head tag.
```html
<!--Inline-->
<body>
<h1 style="color: red;">Inline CSS</h1>
</body>

<!--Internal-->
<head>
    <style>
        h2{color: blue;}
    </style>
</head>
<body>
<h1>Internal CSS</h1>
</body>
```

An `External` CSS file with the **.css** extention linked in the head tag using link tag with the rel and href attributes.
```html
<head>
    <link rel="stylesheet" href="/styles.css">
</head>
```
```css
body{
    background-color: rgb(118, 210, 159);
}
p{
    color: white;
    background-color: rgb(9, 113, 113);
}
```

**SELECTORS** Element selectors, Universal selectors, class name, id name.
```css
/*Element selector*/
h1, p, ...{
    color: red;
}
/*Universal selector*/
*{
    color: red;
}
/*Grouping selectors*/
p,h1,h3{
    color: red;
}
/*Id selector*/
#head1{
    color: green;
}
/*Class selector*/
.para1{
    color: rgb(255, 0, 0);
}
```
```html
<h1 id="head1">Id</h1>
<h1 class="head1">Id</h1>
```

**BORDER**<br>
<img src="images/borders.PNG" alt="border_image" width="30%" height="30%"><br>

```css
h1{
    border: 10px solid blue; /*Shorthand: width style color*/
}
h2{
    border-style: solid;
    border-width: 5px 20px; /*Top and botoom=5px Right and left=20px*/
    border-width: 5px 10px 15px 20px;
    border-color: red blue violet black; /* top=red right=blue bottom=violet left=black*/
}
h3{
    border-left-style: solid;
    border-top-style: dotted;
    border-bottom-style: groove;
    border-right-style: inset;
    border-top-width: 15px;
    border-color: red;
}
h1{
    border: 5px solid blue;
    border-radius: 20px;
}
h2{
    border: 5mm ridge rgba(19, 68, 227, 0.6); /*ridge*/
    border-radius: 20px;
}
p{
    border-style: dotted;
}
```

**MARGIN** Creating space around an element, pushing it away from other elements or browser. Margin set four sides of an element (top,right,bottom,left). Use different units of measurement.
```css
*{
    margin: 0px;
}
h1{
    margin: 80px 40px 20px 10px; /*Top=80 Right=40 Bottom=20 Left=10*/
    
}
h2{
    text-align: right;
    margin-top: 50px;
    margin-bottom: 20px;
    margin-right: 40px;
    margin-left: 80px;
}

```
```html
<div class="margin"><span>MARGIN</span></div>
```

**PADDING**<br>
<img src="images/margin-padding.png" alt="margin-padding_image" width="30%" height="30%"><br>

```css
.padding-h2{
    padding: 20px; /*TOP RIGHT BOTTOM LEFT*/
    padding: 20px 50px; /*TOP=20 BOTTOM=20 RIGHT=50 LEFT=50*/
    padding: 10px 50px 80px; /*TOP=10 RIGHT=50 BOTTOM=80 LEFT=50*/
}
.padding-para{
    padding-top: 10px;
    padding-right: 20px;
    padding-bottom: 40px;
    padding-left: 80px;
}
```

**HEIGHT and WIDTH**<br>
<img src="images/pad-height-width.PNG" alt="height-width_image" width="30%" height="30%"><br>

```css
.height-width-h3{
    border: 5px solid blueviolet;
    width: 250px;
    height: 50px;
}

.height-width-div{
    height: 100px;
    width: 100px;
    background-color: blueviolet;
}
```

**OUTLINE**<br>

<img src="images/outline.PNG" alt="outline_image" width="30%" height="30%"><br>

```css
h4{
    border: 5px solid red;
    outline-style: solid;
    outline-width: 2px;
    outline-color: blue;
    outline-offset: 5px;
}
h5{
    outline: 5px dotted red /*outline shorthand*/
    outline-offset: 5px
}
```
Background Image can put in any element
```css
body{
    background-image: url("/images/cat.jpg");
    background-repeat: no-repeat; /*x, y positions*/
    background-position: top right; /* positions*/
    background-attachment: fixed;/*image fixed, scroll*/
    background-size: cover;
}
```

TEXT<br>
<img src="images/textshadow.PNG" alt="textshadow_image" width="30%" height="30%"><br>

```css
p{
    text-align: center;
    text-decoration: underline;
    text-transform: uppercase;
    text-indent: 30px;
    letter-spacing: 5px;
    line-height: 2;
    word-spacing: 5px;
    text-shadow: 2px 5px 10px black; /*horizontal vertical blur*/
}
```

LIST
```css
list-style-type: square;
list-style-type: upper-alpha; 
ul,ol{
    list-style-position: inside;
}
li{
    border: 1px solid black;
}
```

TABLE<br>
<img src="images/list-table.PNG" alt="list-table_image" width="30%" height="30%"><br>
Table Hoover and Odd<br>
<img src="images/table-hoover-odd.PNG" alt="table-hoover-odd_image" width="30%" height="30%"><br>

```css
table, th,td{
    border: 2px solid black;
    border-collapse: collapse;
}
table{
    width: 100%;
}
th{
    height: 30px;
    vertical-align: middle;
    background-color: blueviolet;
    color: white;
}
td{
    height: 25px;
    text-align: center;
    /* background-color: yellow; */
}
tr:hover{
    background-color: grey; /*hoover tr !No bgc defined at td*/
}
tr:nth-child(odd){
    background-color: yellowgreen; /*Odd-even !No bgc defined at td*/
}
```

OVERFLOW example div text<br>

<img src="images/overflow-problem.PNG" alt="overflow-problem_image" width="30%" height="30%">
<img src="images/overflow-prosolved.PNG" alt="overflow-prosolved_image" width="30%" height="30%"><br>

```css
.overflow{
    background-color: yellowgreen;
    width: 250px;
    height: 200px;
    
    overflow: visible;/*default state*/
    overflow: hidden;/*no overflow*/
    overflow: scroll;/*scroll*/
    overflow: auto; /*default scroll*/
}
```

**ABSOLUTE UNITS & RELATIVE UNITS**<br>
ABSOLUTE UNITS:
`px` (pixels), `cm` (centimeters), `mm` (millimeters), `in` (inches), `pt` (points), `pc` (picas): Also<br>
RELATIVE UNITS:
`em`: Relative to the font size of the element itself.
`rem`: Relative to the font size of the root element (`<html>`).
`%` (percentage): Relative to the parent element's size.
`vw` (viewport width), `vh` (viewport height): Relative to the viewport's dimensions.
`vmin`, `vmax`: Relative to the smaller or larger dimension of the viewport, respectively.
`ch`: Relative to the width of the "0" character.
`ex`: Relative to the x-height of the font.

```html
<div class="div-parent-em">
    <p>Paragraph 1</p>
    <div class="div-chil-em"> <!--child inherit fontsize as below mentioned-->
        <p>Paragraph 2</p>  
    </div>
</div>


.div-parent-em{
    font-size: 20px;
}
```
EM
```css
.div-parent-em{
    font-size: 20px;
}
.div-child-em{
    font-size: 2em; /*child double from parent*/
}
```

**`EM`**<br>
<img src="images/em-relative-unit.PNG" alt="em-relative-unit_image" width="30%" height="30%"><br>

REM
```css
html{
    font-size: 20px;    /*Root value passing through REM EM*/
}
.div-parent-em{
    font-size: 2rem;    /*REM = 2*root */
}
.div-child-em{
    font-size: .5em;    /*.5em half from parent 2rem */
}
```
**VIEWPORT**  is the user's visible area of a web page. Here empty parent child div tag. **PERCENTAGE** relative to the parent element<br>
<img src="images/viewport-percentage.PNG" alt="viewport-percentage_image" width="30%" height="30%"><br>

```css
.div-parent-viewport{
    width: 30vw;
    height: 10vh;
    background-color: blueviolet;
}
.div-child-viewport{
    width: 50%;
    height: 75%;
    background-color: blue;
}

<div class="div-parent-viewport">
    <div class="div-child-viewport">
    </div>
</div>
```
**LINK**
```css
<a href="#" class="link1">Google</a>
<a href="#" class="link2">Facebook</a>
<a href="#" class="link3">Instagram</a>

a{
    color: red;
    text-decoration: none;
    cursor: pointer;
    padding: 10px;
}
a:hover{
    color: black;
    background-color: red;
}
```

**POSITIONS**<br>
1.Static - Default, cant change TOP, BOTTOM, LEFT, RIGHT properties.<br>
2.Rlative - it to be adjusted away from its normal position. `Other content will not be adjusted to fit into any gap left by the element`.<br>
3.Absolute -  is positioned relative to the nearest positioned ancestor, if an absolute positioned element has no positioned ancestors, it uses the document body. `Note: Absolute positioned elements are removed from the normal position, and occupied its position by other elements.`<br>
4.Fixed - is positioned relative to the ***viewport***, which means `it always stays in the same place even if the page is scrolled`. The top, right, bottom, and left properties are used to position the element.<br>
5.Sticky - it must stay within it’s containing block (it’s parent)! `Once that containing block scrolls off the page, it leaves with it`.<br>

<img src="images/positions.PNG" alt="positions_image" width="30%" height="30%"><br>

```css
<div class="parent-position">
    <div class="child-position1">Relative</div>
    <div class="child-position2">Absolute</div>
    <div class="child-position3">Fixed</div>
    <div class="child-position4">Sticky</div>
</div>

.parent-position{
    width: 300px;
    height: 200px;
    border: 2px solid black;
    margin: auto;
    position: relative; /* position to followed by absolute */
}
.child-position1{
    width: 40px;
    height: 40px;
    background-color: blue;
    margin: 2px;
  /*position: static;    Static or default value*/
  /*top: 10px;           any value wont apply Static or default  */
    position: relative;
    left: 40px;
    top: 25px;
}
.child-position2{
    width: 40px;
    height: 40px;
    background-color: green; 
    margin: 2px;
    position: absolute; /* absolute follows parent position or if not body element*/
    top: 0px;
    right: 10px;
}
.child-position3{
    width: 40px;
    height: 40px;
    background-color: yellowgreen;
    margin: 2px;
    position: fixed; /* fixed at viewport */
    left: 10px;
    top: right;
}
.child-position4{
    width: 40px;
    height: 40px;
    background-color: blueviolet;
    margin: 2px;
    position: sticky; /* sticky only from top 0-pixel */
    top: 0px;
}
```

**DISPLAY :**
HTML element has a default display value block or inline. `Block-level` element always starts on a new line and takes up the full width available **(div, h1, p, form, header, footer, section)**. `Inline` element DOES NOT start on a new line and only takes up as much width as necessary **(span, a, img)**.<br>
`The display property has many values!`, ex: inline, block. `display:none`	The element is completely removed, and the page will be displayed as if the element is not there. `visibility:hidden`  The element will be hidden, will still take up the same space as before.<br>

<img src="images/display-elements.PNG" alt="display-element_image" width="30%" height="30%"><br>

```css
img{
    width: 100px;
    height: 100px;
    display: block; /* img element as block */
}
li{
    display: inline; /* li element as inline */
    padding: 10px;
    background-color: blueviolet;
}

 <ul>
        <li>HOME</li>
        <li>ABOUT</li>
        <li>SERVICE</li>
        <li>CONTACT</li>
    </ul>
    <img src="/images/bird1.png" alt="bird1_image">
    <img src="/images/bird2.png" alt="bird2_image">
    <img src="/images/bird3.png" alt="bird3_image">
```

**FONTS**<br>
`Web safe fonts`: always check how your fonts appear on different browsers and devices, and always use fallback fonts; `Fallback Fonts`: If the first font does not work, the browser will try the next one, and the next one, and so on.<br>
Google Fonts (CDN): add a special style sheet link in the `<head>` section and then refer to the font in the CSS. Multiple Google fonts, just separate the font names with a pipe character `(|)`.

```css
h1{
    font-family: Arial, Helvetica, sans-serif; /*web safe fonts & fallback*/
}
@font-face {
    font-family: "montserrat-light";
    src: url(/fonts/Montserrat-Light.ttf); /*downladed font file*/
}
html{
    font-family: "montserrat-light";
}

<link rel="" href="https://fonts.googleapis.com/css?family=Audiowide|Sofia|Trirong"> /*multiple fonts through content delivery network*/ 



```
