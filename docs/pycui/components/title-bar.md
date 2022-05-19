# PYCTitleBar
The title bar component indicates a section of a page.

## Usage
### HTML
```html
<div class="pyc-title-bar">
    <h2 class="pyc-title-bar__title">Title Bar</h2>
</div>
```

### HTML Caveats
You can add an icon to the title bar as a stylistic option.

```html
<div class="pyc-title-bar">
    <i class="pyc-title-bar__icon">
        <!-- Image, SVG, etc. -->
    </i>
    <h2 class="pyc-title-bar__title">Title Bar</h2>
</div>
```

### SCSS
```scss
@use 'node_modules/@pycord/pycui';
@use 'node_modules/@pycord/pycui/pyc-title-bar';

@include pycui.init {
  @include pyc-title-bar.render();
}
```

## API
### CSS Classes
#### Anatomical Classes
| Class Name        | Description                |
|-------------------|----------------------------|
| `pyc-hero`        | The main title bar class.  |
| `pyc-hero__title` | The title bar title class. |
| `pyc-hero__icon`  | The title bar icon class.  |