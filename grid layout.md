# 1. Grid Container
## grid-template-columns Property
-  Define the **number of columns** 
-  Define the **width of each column**
```css
/*4個 column 等寬*/
grid-template-columns: auto auto auto auto;
/*分別不同寬*/
grid-template-columns: 80px 200px auto 40px;
```
## grid-template-rows Property
```
grid-template-rows: 80px 200px;
```
[來源1](https://www.youtube.com/watch?v=lI81W0A-GUc)
[來源2](https://www.w3schools.com/css/css_grid.asp)

透過表格方式來布置元素位置。  
```

<style>
.grid-container {
  display: grid; /*用grid來顯示*/
  grid-template-columns: auto auto auto;
  background-color: #2196F3;
  padding: 10px;
}
.grid-item {
  background-color: rgba(255, 255, 255, 0.8);
  border: 1px solid rgba(0, 0, 0, 0.8);
  padding: 20px;
  font-size: 30px;
  text-align: center;
}
</style>
</head>
<body>


<div class="grid-container">
  <div class="grid-item">1</div>
  <div class="grid-item">2</div>
  <div class="grid-item">3</div>  
  <div class="grid-item">4</div>
  <div class="grid-item">5</div>
  <div class="grid-item">6</div>  
  <div class="grid-item">7</div>
  <div class="grid-item">8</div>
  <div class="grid-item">9</div>  
</div>

</body>
</html>

```
# 2. Grid Item
- By default, a container has **one grid item** for each column and row.
## 2.1 grid-column Property
- Define where the item will start, and where the item will end.
- Note: The grid-column property is a shorthand property for the **grid-column-start** and the **grid-column-end** properties.
- line numbers,  keyword "span" 

```css
/*line numbers*/
.item1 {
  grid-column: 1 / 3;
}
/*grid-column-start: 1;*/
/*grid-column-end: 3;*/
/*-----------------------*/
.item1 {
  grid-column: 1 / span 2;
}
```
## 2.2 grid-row Property
```css
.item1 {
  grid-row: 1 / 4;
}
```
# Grid Lines
<img src = 'https://www.w3schools.com/css/grid_lines.png'>

```
.item1 {
  grid-column-start: 1;
  grid-column-end: 3;
}
```
## 2.3 The grid-area Property
- Shorthand property for the grid-row-start, grid-column-start, grid-row-end and the grid-column-end properties.
![照片](./'擷取.PNG')
