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

    <link rel="stylesheet" type="text/css" href="https://cdn.jsdelivr.net/gh/laws-africa/tausi-web@1.1.0/dist/css/tausi-web.min.css">

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

## Building and releasing

### Building

To build changes:

* npm install
* npm run-script build
* git add dist/*

### Release process

* update version in `package.json`
* update version in URL [above](#from-cdn)
* update version history [below](#version-history)
* build as [above](#building)
* tag release: `git tag vX.X.X`
* push to GitHub: `git push; git push origin --tags`

# Version history

## 1.1.0 (2 November 2021)

* Improved footnote styling

## 1.0.3 (7 October 2021)

* Division and paragraph headings: left-align, reduce font size and line height
* Uppercase extra header text, parties listing
* Match space below republic head to rest of block (remove extra space above authority)

## 1.0.2 (29 September 2021)

* Include changes from previous release in distribution

## 1.0.1 (28 September 2021)

* Uppercase doc-date, judges, docket-number, and doc-authority in the header (in addition to republic-head and decision-action)

## 1.0.0 (27 September 2021)

* Initial release

# License

Proprietary.
