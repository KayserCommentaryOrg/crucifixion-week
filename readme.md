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

<link rel="stylesheet" href="components-build.css">
<script src="bundle.js"></script>
```
