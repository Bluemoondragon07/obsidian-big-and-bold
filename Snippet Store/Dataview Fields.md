# Styled Inline Fields
```css

/* DATAVIEW */

.dataview.inline-field * {
background-color: transparent;
padding: 0px;
}
.dataview.inline-field-standalone-value {
    font-family: inherit;
    color: var(--text-faint);
}
.dataview.inline-field-key {
    background-color: transparent;
    font-family: inherit;
}
.dataview.inline-field-key::after {
    content: '|';
    font-weight: 100;
    color: var(--text-normal);
    padding: 0px 4px;
    font-family: 'Noto Sans Symbols 2', 'Noto Emoji';
}
.dataview.inline-field-value {
    font-family: inherit;
    color: var(--text-faint);
}
```
