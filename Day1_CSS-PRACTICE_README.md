# CSS Day 1 – Basics, Selectors & Text Styling

📅 Date: 27th June 2025  
👩‍💻 Prepared by: Sakshi Aurade

---

## ✅ Topics Covered (With Explanations + Examples)

---

### 🔹 1. What is CSS?

**CSS** stands for **Cascading Style Sheets**.  
It controls the **visual appearance** of HTML content — colors, fonts, layouts, spacing, positioning, responsiveness, and more.

---

### 🔹 2. CSS Syntax

```css
selector {
  property: value;
}
```

🔸 Example:

```css
p {
  color: blue;
  font-size: 16px;
}
```

---

### 🔹 3. Types of CSS

| Type         | Description                       | Example |
|--------------|-----------------------------------|---------|
| **Inline**   | Inside an element’s `style` tag   | `<h1 style="color:red;">Hi</h1>` |
| **Internal** | Inside `<style>` in HTML `<head>` | `<style> p {color:green;} </style>` |
| **External** | Linked `.css` file via `<link>`   | `<link rel="stylesheet" href="style.css">` |

---

### 🔹 4. Colors in CSS

- **Color Names**: `red`, `blue`, `green`
- **RGB Format**: `rgb(255, 0, 0)`
- **Hex Format**: `#ff0000`

```css
body {
  background-color: #f0f0f0;
  color: rgb(50, 50, 50);
}
```

---

### 🔹 5. Common CSS Properties

```css
color: red;
background-color: yellow;
font-size: 18px;
text-align: center;
```

---

### 🔹 6. CSS Selectors

| Selector Type     | Syntax        | Example                     |
|-------------------|---------------|------------------------------|
| Universal         | `*`           | `* { margin: 0; }`           |
| Element Selector  | `tagname`     | `p { font-size: 14px; }`     |
| ID Selector       | `#idName`     | `#title { color: blue; }`    |
| Class Selector    | `.className`  | `.box { padding: 10px; }`    |

---

### 🔹 7. Text Properties

```css
text-align: center;
text-decoration: underline;
font-weight: bold;
font-family: Arial, sans-serif;
line-height: 1.5;
text-transform: uppercase;
```

---

### 🔹 8. Font Families

#### Generic Font Families:
- `serif`
- `sans-serif`
- `cursive`
- `fantasy`
- `monospace`

#### Specific Font Families:
- `"Arial"`
- `"Roboto"`
- `"Times New Roman"`
- `"Georgia"`

```css
p {
  font-family: "Arial", sans-serif;
}
```

---

### 🔹 9. Units in CSS

#### Absolute Units:
- `px` – pixels
- `pt` – points
- `cm`, `mm`, `in` – for print

#### Relative Units:
- `%` – relative to parent
- `em` – relative to parent font size
- `rem` – relative to root font size
- `vw` / `vh` – viewport width/height

---

## 💻 Practice Summary

Created a basic HTML resume-style page and applied:
- Color & background-color
- Font family and text alignment
- All types of selectors
- Tried various units and font weights

---

## 🧠 Note

This README is part of my **Frontend Developer Learning Journey**.  
Will be updated after every day of practice.  
Next: **Box Model, Positioning, and Flexbox**

---
