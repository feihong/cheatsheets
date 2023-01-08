# ImageMagick Cheatsheet

## Install

`brew install imagemagick`

## Resize selfie.jpg so that its width becomes 800px (ratio preserved)

`convert selfie.jpg -resize 800 resized_selfie.jpg`

## Resize input.jpg so that its height becomes 600px (ratio preserved)

`convert input.png -geometry x600 output.png`

## Resize logo.gif, ignoring its original aspect ratio

`convert logo.gif -resize 644x644\! resize_logo.gif`

## Convert an SVG file to PNG

`convert -density 1200 -resize 320x240 test.svg test.png`

## Combine PDF files together, vertically

`convert prefix-1.png prefix-2.png prefix-3.png -append result.png`

## Convert image to black and white

    convert invoice-1.heic -monochrome invoice-1.png
    
More information-preserving

    convert invoice-1.heic -remap pattern:gray50 invoice-1.png

## Sources

- [Resizing or Scaling](http://www.imagemagick.org/Usage/resize/)
