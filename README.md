# CSS Only SASS Masonry Mixin

## Demo
http://codepen.io/doptrois/pen/JoyzKw

## Supports gap indication in
 - Pixels
 - Rems
 - Percentages*

*Percent gaps are not supported by css columns e.g. columns-gap: 3%.
The mixin will simulate that behaviour for you.

Some mixins used from bourbon.io

## How To
your-masonry-container {
    @include masonry(3, 2%, "> *");
}
Each variable is optional. Defaults are shown above.

## Note

If you use percentages for columns gaps, it's recommended to not style the direct child elements of your-masonry-container and wrap the content inside with an additional element and style these elements like in this example.
