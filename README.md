# Tile SVG Specifications

Here is a [Sample SVG file](assets/sample.svg) to download and study.

## Specifications

### `.svg` file extension

File must be a `.svg` file and contain vectors (no raster graphics)

<img src="assets/save-as-svg.jpg" alt="Save as SVG" style="margin-bottom: 25px; width: 150px;" />

### Artboard must be square
Mine are `200x200px`, but any size should be fine as long as it's square.

<img src="assets/dimensions.jpg" alt="Square Artboard" style="margin-bottom: 25px; width: 350px;" />

### All must be shapes must be closed
Use closed shapes only and independant of each other; no groups.

<img src="assets/one-shape-vs-multiple-lines.jpg" alt="One shape" style="margin-bottom: 25px; width: 400px;" />

### All shapes should have a white fill and 0.5px black stroke.

<img src="assets/white-fill-black-stroke.jpg" alt="White fill and black stroke" style="margin-bottom: 25px; width: 400px;" />

### Testing
You can use illustrator to test that the pieces of the tile will work in the React app by giving them a fill color.

<img src="assets/testing-fills.jpg" alt="Testing fills" style="margin-bottom: 25px; width: 400px;" />

It's also a good idea to test that your pattern makes sense by copy/pasting your design to make a 2x2 grid.

<img src="assets/testing-pattern.jpg" alt="Testing fills" style="margin-bottom: 25px; width: 400px;" />

### CSS Properties
__Very important:__ CSS Properties need to be set to "Presentation Attributes" when saving in Adobe Illustrator

<img src="assets/css-props-presentation-attributes.jpg" alt="Presentation attributes" style="margin-bottom: 25px; width: 400px;" />

The reason for this is that illustrator will add the shapes' styles inline on the SVG elements rather than using classes inside a `<style>` tag.

<img src="assets/purpose-of-presentation-attributes.jpg" alt="Presentation attributes" style="margin-bottom: 25px;" />