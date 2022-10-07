## CSS

### CSS Syntax
<img src="https://www.w3schools.com/css/img_selector.gif" alt="css-syntax">


### 1. Inline CSS

`style` attribute is used to define CSS properties at each HTML element.

```html
<h1 style = "color:blue; font-size:40px; font-style: italic;"> One Compiler </h1>
```

### 2. Internal CSS

You can define CSS properties using the `<style>` tag in the `<head>` section.

```html
<head>
    <style>
        body {background-color: pink;}
        h1   {color: red;}
        h2   {color: green; font-size : 40px; font-style: italic;}
    </style>
</head>
```

### 3. External CSS

`<link>` tag is used to refer to an external CSS file.

```html
    <link rel="stylesheet" href="styles.css" />
```

### 4. CSS Selectors

You can select elements based on their name

```css
    div {
        font-familt:'Inter',sans-serrif;
        max-width:400px;
    }
```

or you can use both class based or id based css selection. 

```css
    // classed based 
    .container {
        background:red;
        height:600px;
    }
    // id based
    #container {
        background:purple;
        margin:10px;
    }
```

### 5. FlexBox

You can use Flexbox to manage alignment and position of your elements. 

To use Flexbox, give this property to the parent element:

```css
    .parent {
        display:flex;
    }
```

To align the elements towards the main axis (by default it's horizontal), we use  `justify-content`.

| Vlaues | description |
|---|---|
| flex-start | Items are packed towards the start  | 
| center | Items are packed on the center  | 
| flex-end | Items are packed towards the end  | 
| space-around | Items are equally distributed with equal space aroun them |
| space-between| Items are evenly distributed .first item at the start and last items at the end |
| space-evenly | Items are evenly spaced with same amount space between them | 

To align the elements towards the cross-axis, we use `align-items`.


| Vlaues | description |
|---|---|
| flex-start | Items are packed towards the start of cross axis  | 
| center | Items are packed on the center of cross axis  | 
| flex-end | Items are packed towards the end of the cross axis  | 

By default, the flex direction is set to row (horizontal). To switch the flex direction to column (vertical), use:

### The direction of flex is consider the main axis and the other axis consider as cross axis

```css 
    .parent {
        display:flex;
        flex-direction:column;
    }
```

### 6. CSS Grid
The CSS Grid Layout Module offers a grid-based layout system, with rows and columns, making it easier to design web pages without having to use floats and positioning.

to create a new  grid use  

```css
    .box {
        display:grid;
    }
```

CSS grid is made of two things: columns and rows. Using `grid-template-rows` and `grid-template-columns`, you can define how many rows and columns you want.

```css 
    .box {
        display:grid;
        grid-template-columns:400px 300px 200px;
        grid-template-rows:50px 70px  60px;
    }

```

You can use grid with a special unit called `Fr (fraction)`, which refers to a portion of remaining space.

```css 
    .box {
        display:grid;
        grid-template-columns:1fr 1fr 1fr;
    }
```
