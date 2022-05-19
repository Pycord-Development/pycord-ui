# Pycord UI
A mini-design system for building Pycord projects on the web.

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

## Contributing
If you wish to contribute to this library, please read the [contributing guide](.github/CONTRIBUTING.md).

The [`/packages`](/packages) directory contains the codebase for all Pycord UI implementations.

[`/packages/pycui`](/packages/pycui) is the package for the CSS implementation. The implementation is written in SCSS.

[`/packages/pycui-react`](/packages/pycui-react) is the package for the react implementation. The implementation ~~is~~ will be written in Typescript.

The [`/tests`](/tests) directory contains all the test files for testing the implementations.

## Local Development
Fork and clone the repository
```sh
$ git clone https://github.com/<your-username>/pycord-ui
```

### Installing Dependencies
To install dependencies run the script below in your terminal.
```sh
# NPM
$ npm install

# Yarn
$ yarn
```

### Test building the files (CSS)
To test build the files in the `/tests` directory, run this NPM script in your terminal:
```sh 
# NPM
$ npm run test:sass

# Yarn
$ yarn test:sass
```
This generates `*.css` files for you to check for unexpected behaviors.

### Building the files for distribution (CSS)
To build the files, run this NPM script in your terminal:
```sh 
# NPM
$ npm run test:sass

# Yarn
$ yarn test:sass
```
This generates a `build.css` file in `/packages/pycui/`.