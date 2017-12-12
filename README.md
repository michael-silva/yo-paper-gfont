# yo-paper-gfont
Dialogue box for selecting fonts from [Google Fonts](https://fonts.google.com/)

## Install with bower

First you need bower, [see their site](http://bower.io/) for details 

```
bower install --save yo-paper-gfont
```

## Examples

<!---
```
<custom-element-demo>
  <template>
    <script src="../webcomponentsjs/webcomponents-lite.js"></script>
    <link rel="import" href="yo-paper-gfont.html">
	 <next-code-block></next-code-block>
  </template>
</custom-element-demo>
```
-->
```html
  <yo-paper-gfont google-key="AIzaSyAGvayJHzu-_pbJhTMCO9Fgbz3xjr2qM_g" label="Font label"></yo-paper-gfont>
```
  
## Styling

The following custom properties are available for styling:

| Custom property | Description | Default |
|----------------|-------------|-------------|
| --yo-paper-gfont-font-size | font size of button | 16px |
| --yo-paper-gfont-placeholder-color | color of placeholder | var(--paper-grey-600) |
| --yo-paper-gfont-icon-color | color of check icon |  var(--primary-color) |
| --yo-paper-gfont-label-color | color of button label |  var(--primary-color) |
| --yo-paper-gfont-dialog-width | set the width of change font dialog | 512px |
| --yo-paper-gfont-dialog-min-heigh | set the min-height of change font dialog | 256px |
| --yo-paper-gfont-dialog-max-heigh | set the max-height of change font dialog | 512px |
| --yo-paper-gfont-dialog-background | set the background color of change font dialog | var(--light-theme-background-color) |


## Attributes

### Public

| Attribute Name | Functionality | Type | Default |
|----------------|-------------|-------------|-------------|
| googleKey | always-float-label: boolean label always in float position | boolean  | false |
| placeholder | string to placeholder | string | "Color select" |
| label | string to describe the selected font | string | "Font select" |
| disabled | boolean input diabled | boolean | false |
| readonly | boolean input read only | boolean | false |
| value | string for value of selected font | string | "" |

## Methods

### Private

| Method Name | Action |
|----------------|-------------|
| _dialogHandler(e) | If dialog is confirmed update value |
| _openDialog() | Open dialog if not readonly |
