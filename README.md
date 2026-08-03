# norik.io-demos

Interactive demo blocks from [norik.io](https://norik.io), served at
**https://demos.norik.io**.

Each demo is a folder with an `index.html`. The shared shell adds the common
header, footer, and analytics:

```html
<script src="/shared/shell.js" defer></script>
```

The shell hides its header/footer automatically when a demo is embedded in an
iframe (force with `data-bare`).

## Theme source

`theme/rd-post.css` is the Refracted Descent blog theme from norik.io —
tokens, hero variants, spec-card code blocks, and the browser-window demo
frame.

Each demo folder has a README linking back to the blog post that shares it,
and its `index.html` is self-contained — save the one file and it still works
(the shared shell and webfonts are optional enhancements).
