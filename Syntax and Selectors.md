# CSS Selectors
- select the HTML element(s) you want to style.

## Five categories of CSS selectors:

- Simple selectors (select elements based on **name, id, class**)
- Combinator selectors (select elements based on a specific relationship between them)
- Pseudo-class selectors (select elements based on a certain state)
- Pseudo-elements selectors (select and style a part of an element)
- Attribute selectors (select elements based on an attribute or attribute value)

### 1. by element name (p, a, ...)
```css
p {
  text-align: center;
  color: red;
}
```
### 2. by id (#)
```css
#para1 {
  text-align: center;
  color: red;
}

<p id="para1">Hello World!</p>
```

### 3. by class (.)
```css
.center {
  text-align: center;
  color: red;
}
```
### 4. by element class (_._)
相同class，但指定不同tag
```css
<style>
p.center {
  text-align: center;
  color: red;
}

p.large {
  font-size: 300%;
}
</style>
</head>
<body>

<h1 class="center">This heading will not be affected</h1>
<p class="center">This paragraph will be red and center-aligned.</p>

<!--多重class-->
<p class="center large">This paragraph will be red, center-aligned, and in a large font-size.</p> 

```
### 5. Universal Selector (*)
selects **all** HTML elements on the page.

```css
* {
  text-align: center;
  color: blue;
}
```
### 6. Grouping Selector
```css
h1 {
  text-align: center;
  color: red;
}

h2 {
  text-align: center;
  color: red;
}

p {
  text-align: center;
  color: red;
}
```
當h1, h2, p 有相同style時，可以改寫成以下方式
```css
h1, h2, p {
  text-align: center;
  color: red;
}
```
