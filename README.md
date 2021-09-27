# tausi-web

Web assets (stylesheets) for decisions produced by Tausi.

## Usage

First, wrap your Akoma Ntoso HTML content with the `.akoma-ntoso` class, such as:

```html
<div class="akoma-ntoso">...</div>
```

Second, include the CSS as described below.

### From CDN

Use the assets directly from the [jsDelivr](https://www.jsdelivr.com) CDN:

    <link rel="stylesheet" type="text/css" href="https://cdn.jsdelivr.net/gh/laws-africa/tausi-web@1.0.0/dist/css/tausi-web.min.css">

### From your server

Install @laws-africa/tausi-web using npm:

    $ npm install @laws-africa/tausi-web

Then use either the compiled CSS:

    <link rel="stylesheet" type="text/css" href="tausi-web/dist/css/tausi-web.min.css">

Or use the SCSS files:

    @import 'tausi-web/src/scss/tausi-web';

## Overriding variables

You can override variables when using SCSS by copying them from ``_variables.scss`` into ``_custom.scss`` and changing
their values.

## Building

To build changes:

* npm install
* npm run-scripts build
* git add dist/*

## Release process

* update version in `package.json`
* update version in URL above
* update Version History (below)
* build as above
* tag release: `git tag vX.X.X`
* push to GitHub: `git push; git push origin --tags`

# Version history

## 1.0.0 (27 September 2021)

* Initial release

# License

Proprietary.
