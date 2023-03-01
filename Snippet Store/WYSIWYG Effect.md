# Consistent Line Spacing in both Reading and Editing Modes (A.K.A, a WYSIWYG Effect)

Use this snippet to increase change the line height in both reading and editing modes and make all paragraphs evenly spaced (regardless of whether the `enter` key is pressed once or twice).

>Note: This snippet makes the HTML `<br>` ineffective.

```css

/* -- MAKE PARAGRAPH and LINE SPACING EVEN IN READING AND EDIT MODES */

body {
    --custom-line-height: 2em; /* Experiment with different line heights */
  }

p {
    line-height: var(--custom-line-height) !important;

}

.markdown-preview-view br, .markdown-source-view, br {
    content: '';
    display: block;
    margin-top: calc(var(--custom-line-height) / 2);
}

.markdown-source-view.mod-cm6 .cm-line {
    padding: calc(var(--custom-line-height) / 3) 0px calc(var(--custom-line-height) / 3) 0px;
    line-height: var(--custom-line-height) !important;  
}


/* ---- HEADINGS ------ */
.markdown-rendered h1, .markdown-rendered h2, .markdown-rendered h3, .markdown-rendered h4, .markdown-rendered h5, .markdown-rendered h6 {
    margin: var(--custom-line-height) 0px calc(var(--custom-line-height) * 0.4) 0px !important;
}
.cm-s-obsidian .HyperMD-header {
    padding: var(--custom-line-height) 0px 0px 0px !important;
}

```
