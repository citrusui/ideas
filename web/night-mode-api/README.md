# Night Mode API

If a device or web browser has Night Mode enabled in its settings page, `display-mode` is set to `night`. Otherwise, it is set to `light` or `normal`.

## Concepts

### Dark Mode

```css
@media (display-mode:night) {
  .background {
    background-color: #000;
    color: #fff;
  }
}
```

### Light/Normal Mode

```css
@media (display-mode:light) {
  .background {
    background-color: #fff;
    color: #000;
  }
}
```
