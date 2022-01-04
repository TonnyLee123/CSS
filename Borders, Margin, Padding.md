<img src = 'https://www.w3schools.com/css/box-model.gif'>

# 2. Margin
- Create space around elements, **outside** of any defined borders.
- 控制目前內容在上個內容的相對的位置。
```css
div {
  margin-top: 100px;
  margin-bottom: 100px;
  margin-right: 150px;
  margin-left: 80px;
}
----------上右下左-----------
div {
  padding: 100px 100px 150px 80px;
}
上右下左
-----------全一樣------------
div {
  padding: 25px;
}
```
## The auto Value
```
向右靠齊(把左邊的空間拿走)
margin-left: auto;
--------------------------
置中
margin: auto;
```
# 3. Padding 
- Create space around an element's content, **inside** of any defined borders.

```css
div {
  padding-top: 25px;
  padding-right: 50px;
  padding-bottom: 75px;
  padding-left: 100px;
}
----------上右下左-----------
div {
  padding: 25px 50px 75px 100px;
}
上右下左
-----------全一樣------------
div {
  padding: 25px;
}
```
