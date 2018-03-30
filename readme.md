To launch:

```sh
npm i
npm run build
npm start
```

To rebuild on change:

```sh
npm run watch
```

To deploy:

Run `npm run build`

Copy the `components-build` and `bundle` files from the `public` directory in this folder into whatever place you're deploying.

Add something like this to your HTML:

```html
<div id="target"></div>

<script src="https://cdn.polyfill.io/v2/polyfill.min.js"></script>
<link rel="stylesheet" href="components-build.css">
<script src="bundle.js"></script>
```

You'll need the polyfill.io polyfill for IE11 or whatever.  For `Object.assign`, at least.
