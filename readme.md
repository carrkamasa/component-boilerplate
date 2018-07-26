# Component boilerplate

## Purpose
This boilerplate provides a quick way to build out a reusable component, ready to drop into any project. Out of the box, there is some extremely minimal stlyes, set via a few variables. The idea is that each component build with this boilerplate shouldn't need to touch any styles for fonts, colours etc.

## Features
* Laravel Mix build process (Webpack under the hood)
* Build for dev, production and watch processes
* Extremely minimal boilerplate styling
* Babel JS build process

## Usage
Run the initial build process to install any dependencies
```
$ yarn
```

After the initial ```yarn``` build, there are a few different build commands available (editable via the ```package.json``` file).

Build for dev:
```shell
$ yarn dev
```

Build for production:
```shell
$ yarn production
```

Watch for changes (currently requires a refresh within browser):
```shell
$ yarn watch
```

## Project structure
```shell
themes/your-theme-name/      → Root of your component
├── dist/                    → Compiled resources (never)
│   ├── app.js               → Compiled CSS
│   └── app.css              → Compiled JS
├── img/                     → Any images
├── node_modules/            → Node.js packages (never edit)
├── src/                     → Component uncompiled resources
│   ├── scss/                → Individual scss files
│   ├── app.js               → Uncompiled JS
│   └── app.scss             → Imports scss parts
├── index.html               → Main access point
├── mix-manifest.json        → Paths to compiled files
├── package.json             → Node.js dependencies and scripts
├── webpack.mix.js           → Laravel Mix config
```

## Roadmap
- [x] Initial release
- [ ] Add hot reloading
- [ ] Decide on jQuery dependency by default