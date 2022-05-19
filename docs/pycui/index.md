# Pycord UI (CSS)
The CSS implementation of the Pycord UI

## Purpose
Pycord UI is made to centralize the codebase for Pycord's UI for the web and make all of Pycord's web interfaces
consistent.

## Installation
```sh
# NPM
$ npm install @pycord/pycui sass

# Yarn
$ yarn add @pycord/pycui sass
```

## Instantiation
```scss
@use 'node_modules/@pycord/pycui';

@include pycui.init() {
  // Components go here...
}
```

When instantiating components:

```scss
@use 'node_modules/@pycord/pycui';
@use 'node_modules/@pycord/pycui/pyc-button';

@include pycui.init() {
  @include pyc-button.render();
  ...
}
```

## Components
- [Button](components/button.md)
- [Hero](components/hero.md)
- [Navbar](components/navbar.md)
- [Title Bar](components/title-bar.md)
- [User Card](components/user-card.md)