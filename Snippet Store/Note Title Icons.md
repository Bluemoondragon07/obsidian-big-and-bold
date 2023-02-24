# Note Title Icons

![](Screenshots/icon.png)

This snippet enables you to use icons with any theme! It also comes with customization options you can access with the Style Settings plug-in.

```css
body {
    --icon-emoji: 'Noto Color Emoji';
    --icon-shadow: var(--shadow-ui) inset, var(--shadow-ui);
    --icon-background: var(--background-secondary-alt);
  }
  .icon .inline-title::first-letter {
    font-size: 1em;
    border: 1px solid var(--background-modifier-border);
    border-radius: var(--radius-l);
    margin-right: 0.3em;
    height: auto;
    padding: 15px;
    font-family: var(--icon-emoji);
    font-weight: 500;
    background-color: var(--icon-background);
    box-shadow: var(--icon-shadow);
  }
.icon .inline-title {
    margin-bottom: 0.5em;
    line-height: 2em;
}


/* icon options */

.icon-square .icon .inline-title::first-letter {
    border-radius: 12px;
}
.icon-circle .icon .inline-title::first-letter {
    border-radius: 100px;
    padding: 18px;
}
.icon-bordered .icon .inline-title::first-letter {
    border-radius: 100px;
    border-width: 2px;
    border-color: var(--text-normal);
    padding: 18px;
}
.icon-no-border .icon .inline-title::first-letter {
   border: none;
}


/* @settings

name: Note Title Icons
id: note-title-icons
settings:
    -
        id: icon-style
        title: Icon Style
        type: class-select
        allowEmpty: false
        default: icon-default
        options:
            -
                label: Round
                value: icon-default
            -
                label: Square
                value: icon-square
            -
                label: Circle
                value: icon-circle
            -
                label: Outlined Circle
                value: icon-bordered
    -
        id: icon-emoji
        title: Icon Emoji Style
        type: variable-select
        allowEmpty: false
        default: 'Noto Color Emoji'
        options:
            - 'Noto Color Emoji'
            - 'Noto Emoji'
    -
        id: icon-background
        title: Icon Background
        type: variable-select
        allowEmpty: false
        default: var(--background-secondary-alt)
        options:
            -
                label: Transparent
                value: transparent
            -
                label: Lighter
                value: var(--panel-child)
            -
                label: Pale
                value: var(--background-secondary-alt)
            -
                label: Medium
                value: var(--background-secondary)
            -
                label: Accent
                value: var(--color-accent-2)
    -
        id: icon-shadow
        title: Enable Icon Shadow
        type: variable-select
        allowEmpty: false
        default: var(--shadow-ui) inset, var(--shadow-ui);
        options:
            - 
                label: Inset and Outset
                value: var(--shadow-ui) inset, var(--shadow-ui);
            -
                label: Outset
                value: var(--shadow-ui)
            -
                label: Inset
                value: var(--shadow-ui) inset
            -
                label: None
                value: none
    -
        id: icon-no-border
        title: Remove Icon Border
        type: class-toggle
        default: false
*/

```
