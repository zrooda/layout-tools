[Click here for demo!](http://codepen.io/salsita/full/bgxWBX/)

`npm install iddqd-tools --save`

`@import node_modules/iddqd-tools/sass/all`

```Sass
clearfix
hide-text(true)
truncate(80%)
scrollable(x)
unselectable
aspect-ratio(16, 9)
background-retina('img/bg.png', 250px auto)
abs-fill(0 0 0 50%, 100% auto, -50% 0)
pseudo
em(16)
rem(24)

align(left center, row, 10px)  // Noice!
grid(4, column, 10px, wrap)    // N000ice!!1
```

## align

- align children with Photoshop-like props in either direction converted to flexbox
- emulates internal padding between children

```
+align(<horizontal> <vertical>, row|col|column, <unit>)
// horizontal: left|center|middle|right
// vertical: top|center|middle|bottom
```

## grid

- bidirectional fluid or fixed layout
- spreads children to fit exact row or column space
- emulates internal padding between children

```
+grid(<number> <<number:fixed>, row|col|column, <unit>, wrap|nowrap)
```
