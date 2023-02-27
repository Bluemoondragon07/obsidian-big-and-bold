# Big & Bold Page Gallery
Use this snippet to use **Big & Bold's** style of the page gallery with any theme.

```css
/* -------- PAGE GALLERY --------- */
.page-gallery {
    --gutter-size: var(--custom-gutter-size, 16px);
    --aspect-ratio: var(--custom-aspect-ratio, 1.618);
    --image-width: var(--custom-image-width, calc( (var(--fill-line-width, 700px) - (var(--columns) - 1) * var(--gutter-size)) / var(--columns)));
    --image-height: var(--custom-image-height, calc(var(--aspect-ratio) * var(--image-width)));
    --image-size: var(--custom-image-size, cover);
    --image-position: 50% 75%;
}
.block-language-page-gallery {
    margin: 2em 0px;
    width: 100%;
}
.page-gallery__image, .page-gallery__fallback {
    opacity: 1;
    box-shadow: none;
}
.page-gallery__image:hover, .page-gallery__fallback:hover {
box-shadow: var(--shadow-ui);
}
.page-gallery__fallback {
    background: var(--background-secondary) !important;
}
.page-gallery__tile {
    border: 1px solid var(--background-modifier-border);
    border-radius: var(--radius-m);
    padding: 8px 8px 8px 8px;
    height: flex;
    width: fit-content;
    flex-grow: 1;
    max-width: 20em;
    min-width: 12em;
    background-color: var(--background-secondary-alt);
    box-shadow: var(--shadow-ui);
}
.page-gallery__field {
    text-shadow: none;
    word-wrap: break-word;
    white-space: initial;
    margin-top: 8px;
}
.page-gallery__field a.tag {
    font-size: 0.85em;
}
.page-gallery__field:first-child {
margin-top: 10px;
}
.page-gallery__group-title {
    font-size: var(--h1-size);
    font-family: var(--h1-font);
    text-shadow: none;
    margin: 1em 0px 8px 0px;
}
.page-gallery__filter input {
width: 80%;
}
.page-gallery__filter {
    font-family: 'Noto Emoji';
    font-weight: 900;
    margin-bottom: 2em;
}
.page-gallery__filter-clear {
    filter: none;
    color: var(--text-normal);
    text-decoration: none;
}

```
