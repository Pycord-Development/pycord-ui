# PYCUserCard
The user card component displays information about a user. Use cases include repo contributors, staff pages, etc.

## Usage
### HTML
```html
<div class="pyc-user-card">
    <div class="pyc-user-card__wrap">
        <div class="pyc-user-card__img">
            <img src="#" alt="User avatar" />
        </div>
        <div class="pyc-user-card__info">
            <h3 class="pyc-user-card__name">User name</h3>
            <p class="pyc-user-card__role">Use role</p>
            <p class="pyc-user-card__quote">"Insert quote here"</p>
        </div>
    </div>
    <div class="pyc-user-card__links">
        <a href="#" class="pyc-button is-filled">
            <span class="pyc-button__label">Website</span>
        </a>
    </div>
</div>
```

### SCSS
```scss
@use 'node_modules/@pycord/pycui';
@use 'node_modules/@pycord/pycui/pyc-user-card';

@include pycui.init {
  @include pyc-user-card.render();
}
```

## API
### CSS Classes
#### Anatomical Classes
| Class Name             | Description                          |
|------------------------|--------------------------------------|
| `pyc-user-card`        | The main user card class.            |
| `pyc-user-card__wrap`  | The user card content wrapper class. |
| `pyc-user-card__img`   | The user card image class.           |
| `pyc-user-card__info`  | The user card info section class.    |
| `pyc-user-card__links` | The user card links section class.   |
| `pyc-user-card__name`  | The user card name class.            |
| `pyc-user-card__role`  | The user card role class.            |
| `pyc-user-card__quote` | The user card quote class.           |