# docsify-plugin-giscus

This docsify plugin places giscus as the last child element of `<article class="markdown-section" id="main">`.

[![NPM Version](https://img.shields.io/npm/v/%40mingchyuanko%2Fdocsify-plugin-giscus?style=flat-square)](https://www.npmjs.com/package/@mingchyuanko/docsify-plugin-giscus)

## Usage notes

### Stylesheet

```html
<!-- head -->
<link rel="stylesheet" href="https://unpkg.com/@mingchyuanko/docsify-plugin-giscus/dist/giscus.css">
```

### Script

```html
<!-- body -->
<script src="https://unpkg.com/@mingchyuanko/docsify-plugin-giscus/dist/giscus.min.js"></script>
```

### Configure docsify-plugin-giscus

<https://giscus.app/>

```html
    <script>
        window.$docsify = {
            giscus: {
                repo: "ENTER REPO HERE",
                repoId: "ENTER REPO ID HERE",
                category: "ENTER CATEGORY NAME HERE",
                categoryId: "ENTER CATEGORY ID HERE",
                reactionsEnabled: "1",
                inputPosition: "top",
                theme: "noborder_light",
                lang: "zh-TW",
                loading: true,
            },
        };
    </script>
```

#### theme

- Type: `string`

You can use:

```js
theme: "https://unpkg.com/@mingchyuanko/docsify-plugin-giscus/dist/noborder_light_custom.css",
```

It's just a slight modification of the original file, as there was an issue with the border in the comments section being obscured in the original style.

#### loading

- Type: `boolean`

Loading of the comments will be deferred until the user scrolls near the comments container.
