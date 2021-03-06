---
title: range
subtitle: Slider
type: Widgets
---

A Slider component for displaying current value and intervals in range.

## Notice

- Ingored `exclusiveMinimum`, `exclusiveMaximum`

## API

### schema

Property | Description | Type | Default
-------- | ----------- | ---- | -------
`[minimum]` | The maximum value the slider can slide to	| `number` | -
`[maximum]` | The minimum value the slider can slide to | `number` | -
`[multipleOf]` | The granularity the slider can step through values. Must greater than 0, and be divided by (max - min). When `ui.marks` no null, `step` can be null. | `number` | `1`

### ui

Property | Description | Type | Default
-------- | ----------- | ---- | -------
`[range]` | dual thumb mode | `attribute` | -
`[marks]` | Tick mark of Slider, type of key must be `number`, and must in closed interval `[min, max]` ，each mark can declare its own style. | `object` | -
`[dots]` | Whether the thumb can drag over tick only | `Boolean` | `false`
`[included]` | Make effect when `marks` not null，`true` means containment and `false` means coordinative | `Boolean` | `true`
`[vertical]` | If true, the slider will be vertical | `attribute` | -
`[afterChange]` | Fire when `onmouseup` is fired. | `Function(number[] 丨 number)` | -
`[formatter]` | Slider will pass its value to `nzTipFormatter`, and display its value in Tooltip, and hide Tooltip when return value is null | `Function(value) / null` | -
