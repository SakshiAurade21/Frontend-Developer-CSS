# 🌐 CSS Responsive Design, Transitions, Transforms & Animations

This README covers the concepts learned in Practice Sets 6 & 7 and Level 5 of CSS from Apna College.

---

## 📱 Media Queries (Responsive Design)

Media queries allow us to make our website look good on **all devices** — mobiles, tablets, laptops, desktops — regardless of screen size or orientation.

### ✅ Syntax:
```css
@media (max-width: 600px) {
  div {
    background-color: red;
  }
}
```

### ✅ Example Conditions:
```css
/* Green for width < 300px */
@media (max-width: 299px) {
  div { background-color: green; }
}

/* Pink for 300px to 399px */
@media (min-width: 300px) and (max-width: 399px) {
  div { background-color: pink; }
}

/* Red for 400px to 599px */
@media (min-width: 400px) and (max-width: 599px) {
  div { background-color: red; }
}

/* Blue for width >= 600px */
@media (min-width: 600px) {
  div { background-color: blue; }
}
```

---

## 🔁 CSS Transitions

Transitions allow smooth animation from one CSS state to another (e.g., hover effects).

### ✅ Properties:
- `transition-property`: The CSS property to animate (e.g., `width`, `font-size`, etc.)
- `transition-duration`: How long the animation lasts
- `transition-timing-function`: Controls speed curve (`ease`, `linear`, `ease-in`, etc.)
- `transition-delay`: Delay before transition starts

### ✅ Example:
```css
div {
  transition: font-size 2s ease-in-out 0.2s;
}
```

On `:hover`, `font-size` will grow smoothly.

---

## 🔄 CSS Transform

Used to apply **2D/3D transformations** like rotate, scale, translate, and skew.

### ✅ Rotate
```css
div {
  transform: rotate(45deg);
}
```

### ✅ Scale
```css
transform: scale(1.5);           /* 1.5x both axes */
transform: scaleX(0.5);          /* only X */
transform: scaleY(2);            /* only Y */
transform: scale(1, 2);          /* X and Y separately */
```

### ✅ Translate
```css
transform: translate(20px);       /* right */
transform: translateX(50px);      /* X axis */
transform: translateY(-10px);     /* Y axis up */
transform: translate(20px, 50px); /* X and Y */
```

### ✅ Skew
```css
transform: skew(30deg);           /* Skews both axes */
```

---

## 🎬 CSS Animation

Used to animate elements using keyframes and animation properties.

### ✅ Keyframe Example:
```css
@keyframes growFont {
  from { font-size: 20px; }
  to   { font-size: 40px; }
}
```

### ✅ Using % in Keyframes:
```css
@keyframes growFont {
  0%   { font-size: 20px; }
  50%  { font-size: 30px; }
  100% { font-size: 40px; }
}
```

### ✅ Animation Properties:
- `animation-name`: Name of the keyframe
- `animation-duration`: How long it runs
- `animation-timing-function`: Like transition (`ease`, `linear`, etc.)
- `animation-delay`: Wait time before it starts
- `animation-iteration-count`: Number of times it runs (`infinite` is valid)
- `animation-direction`: `normal`, `reverse`, `alternate`, etc.

### ✅ Shorthand:
```css
animation: growFont 2s linear 3s infinite normal;
```

---

## ✅ Summary

| Topic          | Use                                                |
|----------------|-----------------------------------------------------|
| Media Queries  | Make layouts responsive to screen sizes/orientation |
| Transitions    | Smooth visual effects for changes (hover, focus)    |
| Transforms     | Move/rotate/scale/skew elements                     |
| Animations     | Create movement with keyframes                      |
