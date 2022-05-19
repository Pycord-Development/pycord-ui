# PYCHero
The hero component provides a brief overview of the site contents. It also prompts the user to perform a certain action
to "get them started".

## Usage
### HTML
```html
<section class="pyc-hero">
    <div class="pyc-hero__wrap">
        <img class="pyc-hero__img" src="#" alt="Image" />
        <h1 class="pyc-hero__title">Hero Title</h1>
        <span class="pyc-hero__subtitle">Hero subtitle</span>
        <div class="pyc-hero__actions">
            <a href="#" class="pyc-button is-filled">
                <span class="pyc-button__label">Get Started!</span>
            </a>
        </div>
    </div>
</section>
```

### SCSS
```scss
@use 'node_modules/@pycord/pycui';
@use 'node_modules/@pycord/pycui/pyc-hero';

@include pycui.init {
  @include pyc-hero.render();
}
```

## API
### CSS Classes
#### Anatomical Classes
| Class Name           | Description                     |
|----------------------|---------------------------------|
| `pyc-hero`           | The main hero class.            |
| `pyc-hero__wrap`     | The hero content wrapper class. |
| `pyc-hero__img`      | The hero image class.           |
| `pyc-hero__title`    | The hero title class.           |
| `pyc-hero__subtitle` | The hero subtitle class.        |
| `pyc-hero__actions`  | The hero actions section class. |