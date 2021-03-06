# Basic - Sequence.js Theme

> A basic theme that slides from side to side. A title and subtitle slide in from the top and bottom, and a button appears with a wobble effect

This theme is powered by [Sequence.js](http://sequencejs.com/) - The responsive CSS animation framework for creating unique sliders, presentations, banners, and other step-based applications.

Theme URL: [http://sequencejs.com/themes/basic/](http://sequencejs.com/themes/basic/)


Author: [Ian Lunn](http://ianlunn.co.uk/) - [GitHub](https://github.com/IanLunn) | [Twitter](https://twitter.com/IanLunn) | [Email](mailto:info@sequencejs.com)

## Getting Started

To add a Sequence.js theme to your web page, complete the following:

1. Download and unzip your theme
2. Move the `basic` folder to the same folder as the page you'd like the Sequence.js theme to appear on
3. Add the theme's stylesheet within the `<head></head>` tags on your page, below existing stylesheets. For example:
```html
<link rel="stylesheet" href="basic/css/sequence-theme.basic.css" />
```

4. From `basic/index.html`, copy everything inside the `<body></body>` tags, then paste into the page you'd like the theme to appear on.
5. From `basic/index.html`, copy any `<script></script>` elements found toward the bottom of the page and paste just before the closing `</body>` tag. This should include a reference to the Sequence.js library, its third-party dependencies, and the theme's options, for example:
```html
<script src="basic/scripts/imagesloaded.pkgd.min.js"></script>
<script src="basic/scripts/hammer.min.js"></script>
<script src="basic/scripts/sequence.min.js"></script>
<script src="basic/scripts/sequence-theme.basic.js"></script>
```

6. Save your file and view in the browser. You're done!

### Customizing a Theme

To customize how a theme behaves, its Sequence.js options can be changed in `basic/scripts/sequence-theme.basic.js`. See Options in the [documentation](http://www.sequencejs.com/documentation/#options).

To customize how a theme looks and how its step's transition, refer to the theme's stylesheet: `basic/css/sequence-theme.basic.css`.

It is recommended to read [Setting Up a Theme](http://www.sequencejs.com/documentation/#setting-up-a-theme) in the documentation for an overview of how transitions are applied to Sequence.js steps.

## Using Grunt.js to Develop a Theme

If you are familiar with Grunt.js, you can use it to automate common development tasks. This however is optional and isn't required for a theme to work.

Sequence.js and the themes it powers use [Grunt.js](http://gruntjs.com/) to automate useful tasks. With Grunt.js installed (see Grunt.js' [Getting Started](http://gruntjs.com/getting-started)), use the following command to install this theme's development dependencies:

```
npm install
```

Once development dependencies have installed you can use the commands `grunt serve` and `grunt`.

### `grunt serve`

This command will start a development environment with the following automated tasks:

- Starts a [livereload](http://livereload.com/) session that will reload your browser whenever a file is changed (be sure to install [livereload](http://livereload.com/))
- Opens your browser and navigates to `http://localhost:8000/`
- Sets up a *watch* task to run the following sub-tasks:
  - Update the version number of the following files when changed in `package.json`:
    - `scripts/sequence-theme.basic.js`
    - `scss/sequence-theme.basic.scss`
    - `css/sequence-theme.basic.css`
    - `bower.json`
  - Process any `.scss` files found in the `scss` directory, autoprefix them and then copy to `css` and minify
  - Refresh the browser when any changes are made in HTML, JS, CSS, or SCSS files

You only need to run `grunt serve` per each development session as the *watch* task will continue to operate as you modify files.

### `grunt`

The `grunt` command is a manual version of the *watch* sub tasks listed for the `grunt serve` command.

## Theme License

This theme is made available under a [GPLv3 license](http://sequencejs.com/licenses/#free-theme).

Copyright ?? 2015 [Ian Lunn Design Limited](http://ianlunn.co.uk/)

## Sequence.js License

This theme is powered by [Sequence.js](http://sequencejs.com/). Sequence.js is made available under the following licenses where applicable:

- [GPLv3](http://sequencejs.com/licenses/#personal-open-source-overview) - For personal and open-source projects
- [Commercial License](http://sequencejs.com/licenses/#commercial-overview) - For commercial projects
- [Commercial OEM License](http://sequencejs.com/licenses/#commercial-oem-overview) - For commercial OEM projects
