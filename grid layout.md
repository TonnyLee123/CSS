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
/*設定一個container*/
.grid-container {
  display: grid; /*設定成 grid 模式*/
  grid-template-columns: auto auto auto; /*column數量及寬度(3個, 等寬)*/
  background-color: #2196F3; /*大背景顏色*/
  padding: 20px;/*裡面整體表格與container間的距離*/
}

/*設定裡面的元素*/
.grid-item {
  background-color: rgba(255, 255, 255, 0.8); /*單個元素背景顏色*/
  border: 2px solid rgba(0, 0, 0, 0.8); /*單個元素的邊框*/
  padding: 20px; /*元素內容與邊框之間的距離*/
  font-size: 30px; /*字體*/
  text-align: center; /*裡面的字置中*/
}
</style>

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
- Assign names to grid items.
!(照片)[./'擷取.PNG']
```css
.item8 {
  grid-area: 1 / 2 / 5 / 6;
}
```

## 2.3 grid-template-areas
- Use the **grid-area** to name grid items.
- https://www.w3schools.com/cssref/tryit.asp?filename=trycss_grid-template-areas2
- https://www.w3schools.com/css/tryit.asp?filename=trycss_grid_grid-area_named3
- https://www.w3schools.com/css/tryit.asp?filename=trycss_grid_grid-area_named
