# PYCNavbar
The navbar component lets users navigate the site. The component uses semantic HTML to be accessible to screen readers.

## Usage
### HTML
```html
<nav class="pyc-navbar is-visible">
    <ul class="pyc-navbar__wrap">
        <li class="pyc-navbar__item">
            <a href="#">Home</a>
        </li>
        <li class="pyc-navbar__item">
            <a href="#">About</a>
        </li>
        <li class="pyc-navbar__item">
            <a href="#">GitHub</a>
        </li>
    </ul>
</nav>
```

### SCSS
```scss
@use 'node_modules/@pycord/pycui';
@use 'node_modules/@pycord/pycui/pyc-navbar';

@include pycui.init {
  @include pyc-navbar.render();
}
```

## API
### CSS Classes
#### Anatomical Classes
| Class Name          | Description               |
|---------------------|---------------------------|
| `pyc-navbar`        | The main navbar class.    |
| `pyc-navbar__wrap`  | The navbar wrapper class. |
| `pyc-navbar__item`  | The navbar item class.    |

#### Variant Classes
| Class Name   | Description                       |
|--------------|-----------------------------------|
| `is-visible` | Renders the navbar to be visible. |