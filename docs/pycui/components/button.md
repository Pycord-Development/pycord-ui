# PYCButton
The button component allows the user to execute meaningful actions, or navigate the site's landscape.

## Expected Behavior
Buttons are expected to be clear in intention. They should be easy to understand and use. And are single purpose; they
should only be used for one action.

## Usage
### HTML
```html
<button class="pyc-button">
    <span class="pyc-button__label">Button</span>
</button>
```

### HTML Usage Caveats
The button component mostly relies on the native `<button>` element. However, when being used as hyperlinks, we advise you to use the `<a>` element instead.

```html
<!-- In a form context, this is okay... -->
<button class="pyc-button">
    <span class="pyc-button__label">Button</span>
</button>

<!-- 
  ~ However, when using it as a hyperlink, 
  ~ use the anchor tag 
-->
<a href="#" class="pyc-button">
    <span class="pyc-button__label">Button</span>
</a>
```

And whenever the hyperlink leads to an external page, it is advised to use the `target="_blank"` attribute.

```html
<a href="https://google.com" class="pyc-button" target="_blank">
    <span class="pyc-button__label">Button</span>
</a>
```

### SCSS
```scss
@use 'node_modules/@pycord/pycui';
@use 'node_modules/@pycord/pycui/pyc-button';

@include pycui.init {
  @include pyc-button.render();
}
```

## Variants
### Text
This button variant is used for actions that require the minimum amount of attention, or not much attention at all.

This is the default styling of the button when the main button class is applied.

```html
<button class="pyc-button">
    <span class="pyc-button__label">Button</span>
</button>
```

### Outlined
This button variant is used for actions that are an alternative to the primary action (filled variant). 

To apply the styles, append the `is-outlined` class to the main button class.

```html
<button class="pyc-button is-outlined">
    <span class="pyc-button__label">Button</span>
</button>
```

### Filled
This button variant is used for actions that are the first recommended solution. These buttons are the forefront of the
actions, henceforth it is designed to catch the user's attention first.

To apply the styles, append the `is-filled` class to the main button class.

```html
<button class="pyc-button is-filled">
    <span class="pyc-button__label">Button</span>
</button>
```

## API
### CSS Classes
#### Anatomical Classes
| Class Name          | Description             |
|---------------------|-------------------------|
| `pyc-button`        | The main button class.  |
| `pyc-button__icon`  | The button icon class.  |
| `pyc-button__label` | The button label class. |

#### Variant Classes
| Class Name    | Description                               |
|---------------|-------------------------------------------|
| `is-outlined` | Renders the button in its outlined style. |
| `is-filled`   | Renders the button in its outlined style. |
| `is-inverted` | Renders the button in its inverted style. |