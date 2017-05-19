# \<l2t-paper-rating\>

A polymer element to display &#34;star&#34; ratings in a paper style

## Install with bower

First you need bower, [see their site](http://bower.io/) for details

```
bower install --save l2t-paper-rating
```

## Examples

Each slide must be within a paper-slide tag, but other than that you have complete control.
<!---
```
<custom-element-demo>
  <template>
    <script src="../webcomponentsjs/webcomponents-lite.js"></script>
    <link rel="import" href="l2t-paper-rating.html">
	 <next-code-block></next-code-block>
  </template>
</custom-element-demo>
```
-->
```html
  <l2t-paper-rating rating="7" total="10"></l2t-paper-rating>
```

## Styling

The following custom properties are available for styling:

| Custom property | Description | Default |
|----------------|-------------|-------------|
| --rating-icon-color | The color of the icons | #455a64 |
| --rating-icon-size | The size of the icon (square) | 28px |
| --rating-icon-padding | The size of the padding between icons | 2px |
| --rating-unselected-opacity | The opacity of stars 'non-active' | 0.4 |

### Public

| Attribute Name | Functionality | Type | Default |
|----------------|-------------|-------------|-------------|
| icon | the icon to use (iron-icons) | String | icon |
| rating | numbers of star selected (reflectToAttribute) | Number | 1 |
| readonly | can the rate be modified | Boolean | false |
| total | maximum number of stars selectable | Number | 5 |

### Private

| Attribute Name | Functionality | Type | Default |
|----------------|-------------|-------------|-------------|
| _stars | array hack for dom repeat from number | Array | [] |
