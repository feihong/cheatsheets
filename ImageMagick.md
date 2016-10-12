Install: 

`brew install imagemagick`

Resize selfie.jpg so that its width becomes 800px. Ratio is preserved.

```
convert selfie.jpg -resize 800 resized_selfie.jpg
```

Convert an SVG file to PNG:

```
convert -density 1200 -resize 320x240 test.svg test.png
```
