# CSS Only SASS Masonry Mixin

## Demo on codepen.io
http://codepen.io/doptrois/pen/JoyzKw

## Supports gap indication in
 - Pixels
 - Rems
 - Percentages*

*Percent gaps are [not supported by css columns](http://www.w3.org/TR/css3-multicol/#column-gap0) e.g.
```css
columns-gap: 3%
```
The mixin will simulate that behaviour for you.

Some mixins used from [bourbon.io](http://bourbon.io/)

## How To
```scss
your-masonry-container {
    @include masonry(3, 2%, "> *");
}
```
Each variable is optional. Defaults are shown above.

## Note

If you use percentages for columns gaps, it's recommended to not style the direct child elements of 'your-masonry-container' and wrap the content inside with an additional element and style these elements like in the [codepen example](http://codepen.io/doptrois/pen/JoyzKw).
