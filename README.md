> Anticipate the difficult by managing the easy. - Phu K. C'Eses

[Click here for demo!](http://codepen.io/salsita/full/bgxWBX/)

`npm install layout-tools --save`

`@import node_modules/layout-tools/sass/all`

## align

- align children with Photoshop-like props in either direction converted to flexbox
- emulates internal padding between children

```Sass
+align(<horizontal> <vertical>, row(default)|col|column, <unit>)

// horizontal: left|center|middle|right
// vertical: top|center|middle|bottom

// Example
.container
  +align(right center, col, 10px)
```

## grid

- bidirectional fluid or fixed layout
- spreads children to fit exact row or column space
- emulates internal padding between children

```Sass
+grid(<number> <?number:fixed>, row(default)|col|column, <unit>, wrap(default)|nowrap)

// Example
.container
  +grid(4, row, 20px)

  @media (max-width: 640px)
    +grid(1 2.5, col, 10px, nowrap)
```

## other

- [clearfix](sass/clearfix.sass)
- [hide-text](sass/hide-text.sass)
- [truncate](sass/truncate.sass)
- [scrollable](sass/scrollable.sass)
- [unselectable](sass/unselectable.sass)
- [aspect-ratio](sass/aspect-ratio.sass)
- [background-retina](sass/background-retina.sass)
- [abs-fill](sass/abs-fill.sass)
- [pseudo](sass/pseudo.sass)
- [em, rem](sass/em-rem.sass)
