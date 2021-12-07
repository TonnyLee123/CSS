###  Position
- Specify the type of positioning method used for an element (static, relative, fixed, absolute or sticky).
- 1. static (default.)
- 2. not affected by the top, bottom, left, and right properties.
- 3. not positioned in any special way; it is always positioned according to the normal flow of the page
```
position: static;
```

2. relative
- relative to its normal position.

Setting the top, right, bottom, and left properties. 
Other content will not be adjusted to fit into any gap left by the element.
```
position: relative;
left: 20px;
```

3. fixed
- positioned relative to the **viewport**, which means it always stays in the **same place** even if the page is scrolled. 
A fixed element does not leave a gap in the page where it would normally have been located.
```
```
4. absolute
is positioned relative to the nearest positioned ancestor (instead of positioned relative to the viewport, like fixed).

However; if an absolute positioned element has no positioned ancestors, it uses the document body, and moves along with page scrolling.

Note: Absolute positioned elements are removed from the normal flow, and can overlap elements.
