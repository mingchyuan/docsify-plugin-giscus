# docsify-plugin-giscus

This docsify plugin places giscus as the last child element of `<article class="markdown-section" id="main">`.

[![NPM Version](https://img.shields.io/npm/v/%40mingchyuanko%2Fdocsify-plugin-giscus?style=flat-square)](https://www.npmjs.com/package/@mingchyuanko/docsify-plugin-giscus)

## Usage notes

### Stylesheet

```html
<!-- head -->
<link rel="stylesheet" href="">
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

#### loading

- Type: `boolean`

Loading of the comments will be deferred until the user scrolls near the comments container.
