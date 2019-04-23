---
title: Checkbox React component
components: Checkbox, FormControl, FormGroup, FormLabel, FormControlLabel
---

# Kontrollkästchen

<p class="description">Checkboxes allow the user to select one or more items from a set.</p>

Kontrollkästchen können verwendet werden, um eine Option ein- oder auszuschalten.

Wenn in einer Liste mehrere Optionen erscheinen, können Sie durch Kontrollkästchen die Abstände erhalten statt Ein- / Aus - Schalter zu verwenden. Wenn Sie nur eine Option haben, vermeiden Sie die Verwendung eines Kontrollkästchens und verwenden Sie stattdessen einen Ein- / Ausschalter.

{{"demo": "pages/demos/checkboxes/Checkboxes.js"}}

Die `Checkbox` kann dank der `FormControlLabel` Komponente auch mit einer Etikettenbeschreibung verwendet werden.

{{"demo": "pages/demos/checkboxes/CheckboxLabels.js"}}

## Kontrollkästchen mit FormGroup

`FormGroup` ist ein hilfreicher Wrapper zum Gruppieren von Auswahlsteuerungskomponenten, welcher eine einfachere API bietet.

{{"demo": "pages/demos/checkboxes/CheckboxesGroup.js"}}

## Etikettenplatzierung

Sie können die Platzierung des Etiketts ändern:

{{"demo": "pages/demos/checkboxes/FormControlLabelPosition.js"}}

## Barrierefreiheit

Alle Formularsteuerelemente sollten Beschriftungen haben. Dazu gehören Optionsfelder, Kontrollkästchen und Schalter. In den meisten Fällen wird dazu das Element `<label>` ([FormControlLabel](/api/form-control-label/)) verwendet.

Wenn ein Label nicht verwendet werden kann, muss der Eingabekomponente ein Attribut direkt hinzugefügt werden. In diesem Fall können Sie das zusätzliche Attribut (z. B. `aria-label`, `aria-labelby`, `title`) über die Eigenschaft `inputProps` anwenden.

```jsx
<Checkbox
  value="checkedA"
  inputProps={{ 'aria-label': 'Checkbox A' } }
/>
```

## Anleitung

- [Checkboxes vs. Optionsfeld (Radio Buttons)](https://www.nngroup.com/articles/checkboxes-vs-radio-buttons/)