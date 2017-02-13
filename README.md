> Anticipate the difficult by managing the easy. - Phu K. C'Eses

High polish expressive mixins for CSS layout authors, available as a bundle or separately.

[Click here for demo!](http://codepen.io/salsita/full/bgxWBX/)

`npm install layout-tools --save`

`@import node_modules/layout-tools/sass/all`

## align

- expressive wrapper over flexbox
- aligns children inside parent with Photoshop-like props in either direction
- emulates internal padding between children

`+align(<horizontal> <vertical>, <spacing>, <direction>)`

```Sass
// horizontal: left(default)|center|middle|right
// vertical: top(default)|center|middle|bottom
// spacing: unit(default 0)
// direction: row(default)|col|column

// Example
.container
  +align(right center, 10px, col)
```

## grid

- bidirectional fluid or fixed layout
- spreads children to fit exact row or column space
- emulates internal padding between children

``

`+grid(<items-x> <?items-y>, <spacing>, <direction>, <wrap>)`

```Sass
// spacing: unit(default 0)
// direction: row(default)|col|column
// wrap: wrap(default)|nowrap

// Example
.container
  +grid(4, 20px)

  @media (max-width: 640px)
    +grid(1 2.5, col, 10px, nowrap)
```

## abs

- expressive wrapper over absolute positioning
- automatic transform offset for centering
- bidirectional fill with automatic sizing that accepts distance off vertical/horizontal screen edges

`+abs(<horizonal> <?vertical>)`

```Sass
// horizontal: left(default)|center|middle|right|fill or unit
// vertical: top(default)|center|middle|bottom|fill or unit

+abs(50% center)
+abs(right center)
+abs(right 20px fill)
+abs(fill 50px fill)
+abs(center bottom 5px)
+abs(right 30% top 20px bottom)
```

## other

- [clearfix](sass/clearfix.sass)
- [hide-text](sass/hide-text.sass)
- [truncate](sass/truncate.sass)
- [scrollable](sass/scrollable.sass)
- [unselectable](sass/unselectable.sass)
- [aspect-ratio](sass/aspect-ratio.sass)
- [background-retina](sass/background-retina.sass)
- [pseudo](sass/pseudo.sass)
- [em, rem](sass/em-rem.sass)
