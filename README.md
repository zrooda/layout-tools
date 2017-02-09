> Anticipate the difficult by managing the easy. - Phu K. C'Eses

[Click here for demo!](http://codepen.io/salsita/full/bgxWBX/)

`npm install iddqd-tools --save`

`@import node_modules/iddqd-tools/sass/all`

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
+grid(<number> <?number:fixed>, row|col|column, <unit>, wrap|nowrap)
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
