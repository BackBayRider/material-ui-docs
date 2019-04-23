---
title: Radio buttons React component
components: Radio, RadioGroup, FormControl, FormLabel, FormControlLabel
---

# Radio buttons

<p class="description">Radio buttons allow the user to select one option from a set.</p>

当用户需要查看所有可用选项时, 请使用单选按钮。 如果可用选项可以折叠，请考虑使用占用空间更少的下拉菜单。

单选按钮在一般默认选中最常用的选项。

`RadioGroup `适用于一组` Radio `，它提供相对简单的 API 并且能够使用键盘对该RadioGroup进行控制。

{{"demo": "pages/demos/radio-buttons/RadioButtonsGroup.js"}}

## 独立的单选按钮

`Radio` 也可以单独使用，无需额外包装。

{{"demo": "pages/demos/radio-buttons/RadioButtons.js"}}

## 标签放置

你可以更改标签放置的位置:

{{"demo": "pages/demos/radio-buttons/FormControlLabelPosition.js"}}

## 无障碍功能

所有表单控件都应该有标签，这包括单选按钮，复选框和开关。 在大多数情况下，这是通过使用 `<label>` 元素（[FormControlLabel](/api/form-control-label/)）完成的。

如果无法使用标签，则必须直接向输入组件添加属性。 在这种情况下，可以应用附加的属性（例如 `arial-label`， `aria-labelledby`， `title`）经由 `inputProps` 属性。

```jsx
<RadioButton
  value="radioA"
  inputProps={{ 'aria-label': 'Radio A' } }
/>
```

## Guidance

- [Checkboxes vs. 单选按钮](https://www.nngroup.com/articles/checkboxes-vs-radio-buttons/)