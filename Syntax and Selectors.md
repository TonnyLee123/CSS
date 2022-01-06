<img src = 'https://www.w3schools.com/css/img_selector.gif'>


# CSS Selectors
- select the HTML element(s) you want to style.

## Five categories of CSS selectors:

- Simple selectors (select elements based on **name, id, class**)
- Combinator selectors (select elements based on a specific relationship between them)
- Pseudo-class selectors (select elements based on a certain state)
- Pseudo-elements selectors (select and style a part of an element)
- Attribute selectors (select elements based on an attribute or attribute value)

### 1. by tag (p, a, ...)
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

<h1 class="center">Red</h1>
```
### 4. by tag and class (_._)
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

### 7. ::before
Insert some text before the content of each speccify element(tag)
```css

<!--新增content(Read this -) before tag p-->
p::before {
  content: "Read this -";
}

<h1>Demo of the ::before selector</h1>
<p>My name is Donald</p>
<p>I live in Ducksburg</p>

```
### 8.<a href = 'https://www.w3schools.com/cssref/tryit.asp?filename=trycss_sel_after'> ::after</a>
Insert some text after the content of each speccify element(tag)
```css
p::after { 
  content: " - Remember this";
}
```
### 9. :root
- 最多的應用多是搭配 CSS 變數
- 建立變數
```css
1. 整個頁面中都可以使用這個變數(:root)。
2. --csscoke-red 變數名稱 ( --作為開頭)

:root {
	--csscoke-red: #f00;
}
--------------------------------------
1. 某個區域中使用
.section-item {
	--csscoke-title-red: #f00;
}
```
- 套用變數
```
屬性值:var(變數名稱)

.section-item {
	color: var( --csscoke-red );
}
```
