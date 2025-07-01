# 📘 CSS Layout & Visual Concepts (Day Summary)

## 1. 🖼 Display Property

The `display` property defines how an element is displayed on the page.

* `block`: Starts on a new line, takes up full width. (e.g., `<div>`, `<p>`)
* `inline`: Sits beside other elements, only takes space needed. (e.g., `<span>`, `<a>`)
* `inline-block`: Like inline, but allows setting width, height.
* `none`: Hides the element completely.

**Example:**

```html
<div style="display: block;">I'm block</div>
<span style="display: inline;">I'm inline</span>
```

---

## 2. 📦 Block vs Inline Elements

* **Block**: Takes full width. You can set width/height. Starts on a new line.
* **Inline**: Only takes space as per content. Cannot set width/height directly.

**Example:**

```html
<p>This is a block</p>
<span>This is inline</span>
```

---

## 3. 👀 Visibility Property

* `visibility: visible`: Default. Element is shown.
* `visibility: hidden`: Element is invisible but still takes space.

**Example:**

```html
<p style="visibility: hidden;">You can't see me, but I take space!</p>
```

---

## 4. 📏 Units in CSS

### I. % (Percentage)

Used relative to parent element.
**Example:**
If parent is 100px wide, child with width `30%` will be 30px.

```css
div.child {
  width: 30%;
}
```

### II. em

Relative to the font size of the parent element.
**Example:**
If parent font-size is 16px, `1em = 16px`, `2em = 32px`.

```css
p {
  font-size: 2em; /* 32px if parent is 16px */
}
```

### III. rem

Relative to the root (`<html>`) font-size.
**Example:**
If root font-size is 16px, then `2rem = 32px`.

```css
h1 {
  font-size: 2rem; /* 32px */
}
```

### IV. vh (Viewport Height)

1vh = 1% of the browser window height.

```css
.banner {
  height: 50vh; /* Half of screen height */
}
```

### V. vw (Viewport Width)

1vw = 1% of browser window width.

```css
.container {
  width: 100vw; /* Full screen width */
}
```

---

## 5. 📍 CSS Positioning

### static

Default position. Not affected by top/right/bottom/left.

```css
box { position: static; }
```

### relative

Element moves relative to its normal position.

```css
div {
  position: relative;
  top: 10px; /* Moves 10px down from its spot */
}
```

### absolute

Element is positioned relative to the **nearest positioned ancestor** (not static).

```css
.box {
  position: absolute;
  top: 0;
  left: 0;
}
```

### fixed

Positioned relative to the browser window.

```css
.fixed-header {
  position: fixed;
  top: 0;
  width: 100%;
}
```

### sticky

Sticks to a position while scrolling until a certain point.

```css
.sticky-bar {
  position: sticky;
  top: 0;
}
```

---

## 6. 🔢 Z-index

Controls stack order (what shows on top).
Higher `z-index` means it appears above.

```css
.box1 {
  position: absolute;
  z-index: 2;
}
.box2 {
  position: absolute;
  z-index: 1;
}
```

---

## 7. 🖼 Background Image

Set an image as background of a div.

```css
.hero {
  background-image: url('image.jpg');
  background-repeat: no-repeat;
  background-position: center;
}
```

---

## 8. 🎨 Background Size

* `cover`: Cover entire area (may crop)
* `contain`: Fit image completely (may leave space)
* `auto`: Default image size

**Example:**

```css
.hero {
  background-size: cover;
}
```

---

✨ You’ve covered a LOT today — great job! Let me know when you’re ready for Flexbox or next level styling! 💪🚀
