```html
<!DOCTYPE html>
<html lang="fr">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>CSS</title>
    <style>
        h2{color: blue;}
    </style>
    <link rel="stylesheet" href="/styles.css">
</head>
<body>
    <h1 style="color: red;">Inline CSS</h1>
    <p>Lorem ipsum dolor sit amet consectetur, adipisicing elit. Possimus, obcaecati fugiat!</p>
    <h1 id="head1">Id</h1>
    <p class="para1">Lorem ipsum</p>

</body>
</html>
```

```css
body{background-color: rgb(118, 210, 159);}
p{color: white; background-color: rgb(9, 113, 113);}

*{color: red; text-align: center;}

p,h1,h3{
    color: red;
}

```


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

