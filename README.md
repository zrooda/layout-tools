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
- keywords `center|middle` with automatic transform offset fix
- keyword `fill` that accepts distance off screen edges
- shorthands (`center`, `25px`, `fill`, `fill 10px`)
- configurable flow of orientation, default `left top right bottom`
- circular and conflict detection

`+abs(<left|vertical> <top|horizontal> <?right> <?bottom>)`

```Sass
+abs(50%)
+abs(fill 15px)
+abs(right center)
+abs(right 20px fill)
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
