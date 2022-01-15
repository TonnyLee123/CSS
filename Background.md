#  background-size
```css
background-size: 300px 100px;
                 width high
```
- 覆蓋整個container，可能會拉長照片
```css
background-size:cover;
```

# background-repeat
重複照片
https://www.w3schools.com/cssref/playit.asp?filename=playcss_background-repeat&preval=no-repeat
```html
<!DOCTYPE html>
<html>
<head>
<meta name="viewport" content="width=device-width, initial-scale=1">
<style>
body {
  margin:0;
  font-family: Arial, Helvetica, sans-serif;
}

.hero-image {
  background-image: url("/w3images/photographer.jpg");
  background-color: #cccccc;
  height: 500px;
  background-position: center;
  background-repeat: no-repeat;
  background-size: cover;
  position: relative; /*目的: 讓裡面元素有其他position(如下方absolute)*/
}

.hero-text {
  text-align: center;
  position: absolute;
  top: 50%;
  left: 50%; /*當縮小螢幕 讓內容維持原位*/
  transform: translate(-50%, -50%);
  color: white;
}
</style>
</head>
<body>

<div class="hero-image">
  <div class="hero-text">
    <h1 style="font-size:50px">I am Jane Doe</h1>
    <h3>And I'm a Photographer</h3>
    <button>Hire me</button>
  </div>
</div>

<p>Page content..</p>
<p>Note that this technique will also make the image responsive: Resize the browser window to see the effect.</p>

</body>
</html>

```
