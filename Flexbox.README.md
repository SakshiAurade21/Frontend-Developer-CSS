# 💪 CSS Flexbox (Flexible Box Layout)

Flexbox is a **one-dimensional layout system** used to arrange items in **rows or columns**. It makes alignment, spacing, and distribution of elements easier inside a container.

---

## 🔹 The Flex Model

To use Flexbox:
```css
.container {
  display: flex;
}
```

This makes the container a **flex container**, and all its children become **flex items**.

- **Main Axis**: The primary direction (row or column)
- **Cross Axis**: The opposite direction

---

## 🔸 Flex Direction (Main Axis Control)

Controls the direction in which items are placed:

```css
flex-direction: row;           /* Default → Left to right */
flex-direction: row-reverse;   /* Right to left */
flex-direction: column;        /* Top to bottom */
flex-direction: column-reverse;/* Bottom to top */
```

---

## 🔸 Properties for Flex Container

### ✅ `justify-content` → Align items on the **main axis** (horizontal by default)

```css
justify-content: flex-start;   /* Left */
justify-content: flex-end;     /* Right */
justify-content: center;       /* Center */
justify-content: space-between;/* Equal space between */
justify-content: space-around; /* Space around */
justify-content: space-evenly; /* Equal space all sides */
```

---

### ✅ `align-items` → Align items on the **cross axis** (vertical by default)

```css
align-items: stretch;          /* Default */
align-items: flex-start;       /* Top */
align-items: flex-end;         /* Bottom */
align-items: center;           /* Center vertically */
```

---

### ✅ `flex-wrap` → Whether items should wrap to the next line

```css
flex-wrap: nowrap;       /* Default – no wrapping */
flex-wrap: wrap;         /* Items wrap to next line if needed */
flex-wrap: wrap-reverse; /* Wrap in reverse direction */
```

---

### ✅ `align-content` → Align multiple rows (if wrapping)

```css
align-content: flex-start;
align-content: flex-end;
align-content: center;
align-content: space-around;
align-content: space-between;
align-content: space-evenly;
```

📝 *Note: `align-content` only applies when there are multiple rows (with wrapping).*

---

## 📌 Example Layout

```html
<div class="container">
  <div class="box">1</div>
  <div class="box">2</div>
  <div class="box">3</div>
</div>
```

```css
.container {
  display: flex;
  flex-direction: row;
  justify-content: center;
  align-items: center;
}
.box {
  width: 100px;
  height: 100px;
  background-color: pink;
  margin: 10px;
}
```

---

## 🌟 Summary (Flexbox Today)

| Property         | Purpose                             |
|------------------|-------------------------------------|
| `display: flex`   | Activate Flexbox                   |
| `flex-direction`  | Set main axis direction            |
| `justify-content` | Align items on main axis           |
| `align-items`     | Align items on cross axis          |
| `flex-wrap`       | Allow wrapping to new lines        |
| `align-content`   | Align wrapped rows on cross axis   |
