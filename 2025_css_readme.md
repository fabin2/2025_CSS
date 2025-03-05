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
