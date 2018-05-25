[![Published on webcomponents.org](https://img.shields.io/badge/webcomponents.org-published-blue.svg)](https://www.webcomponents.org/element/Link2Twenty/l2t-paper-rating)
[![Published on Vaadin  Directory](https://img.shields.io/badge/Vaadin%20Directory-published-blue.svg)](https://vaadin.com/directory/component/Link2Twentyl2t-paper-rating)
[![Stars on vaadin.com/directory](https://img.shields.io/vaadin-directory/star/Link2Twentyl2t-paper-rating.svg)](https://vaadin.com/directory/component/Link2Twentyl2t-paper-rating)

# \<l2t-paper-rating\>

A polymer element to display &#34;star&#34; ratings in a paper style

## Install with bower

First you need bower, [see their site](http://bower.io/) for details

```
bower install --save l2t-paper-rating
```

## Examples

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
  <l2t-paper-rating></l2t-paper-rating> <br/>
  <l2t-paper-rating rating="2" readonly></l2t-paper-rating> <br/>
  <l2t-paper-rating rating="3" total="4"></l2t-paper-rating>
```

## A11y/ARIA

For screen readers it's helpful to have a label though the traditional label element will not work with custom elements so we'll need to change the [aria-label](https://www.w3.org/TR/WCAG20-TECHS/ARIA14.html) or [aria-labelledby](https://www.w3.org/TR/WCAG20-TECHS/ARIA7.html) properties directly.

There are examples of both methods on the [demo page](https://www.webcomponents.org/element/Link2Twenty/l2t-paper-rating/demo/demo/index.html).

## Styling

The following custom properties are available for styling:

| Custom property | Description | Default |
|----------------|-------------|-------------|
| --rating-icon-color | The color of the icons | --primary-text-color |
| --rating-icon-size | The size of the icon (square) | 28px |
| --rating-icon-padding | The size of the padding between icons | 2px |
| --rating-ink-color | The color of the ripple on icon tap | --primary-text-color |
| --rating-unselected-opacity | The opacity of stars 'non-active' | 0.4 |

## Properties

### Public

| Attribute Name | Functionality | Type | Default |
|----------------|-------------|-------------|-------------|
| icon | the icon to use (iron-icons) | String | star |
| rating | numbers of star selected (reflectToAttribute) | Number | 1 |
| readonly | can the rate be modified | Boolean | false |
| total | maximum number of stars selectable | Number | 5 |
