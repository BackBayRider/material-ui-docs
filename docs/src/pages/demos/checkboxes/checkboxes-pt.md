---
title: Checkbox React component
components: Checkbox, FormControl, FormGroup, FormLabel, FormControlLabel
---

# Caixas de Seleção

<p class="description">Checkboxes allow the user to select one or more items from a set.</p>

Checkboxes can be used to turn an option on or off.

If you have multiple options appearing in a list, you can preserve space by using checkboxes instead of on/off switches. If you have a single option, avoid using a checkbox and use an on/off switch instead.

{{"demo": "pages/demos/checkboxes/Checkboxes.js"}}

`Checkbox` can also be used with a label description thanks to the `FormControlLabel` component.

{{"demo": "pages/demos/checkboxes/CheckboxLabels.js"}}

## Checkboxes with FormGroup

`FormGroup` is a helpful wrapper used to group selection controls components that provides an easier API.

{{"demo": "pages/demos/checkboxes/CheckboxesGroup.js"}}

## Label placement

You can change the placement of the label:

{{"demo": "pages/demos/checkboxes/FormControlLabelPosition.js"}}

## Acessibilidade

All form controls should have labels, and this includes radio buttons, checkboxes, and switches. In most cases, this is done by using the `<label>` element ([FormControlLabel](/api/form-control-label/)).

When a label can't be used, it's necessary to add an attribute directly to the input component. In this case, you can apply the additional attribute (e.g. `aria-label`, `aria-labelledby`, `title`) via the `inputProps` property.

```jsx
<Checkbox
  value="checkedA"
  inputProps={{ 'aria-label': 'Caixa de seleção A' } }
/>
```

## Guidance

- [Checkboxes vs. Butões de Rádio](https://www.nngroup.com/articles/checkboxes-vs-radio-buttons/)