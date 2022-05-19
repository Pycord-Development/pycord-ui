# Developing Pycord UI (CSS)
Below is a guide on developing Pycord UI.

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