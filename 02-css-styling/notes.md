# 🎨 CSS Mastery Notes

## ✅ What is CSS?
- CSS (Cascading Style Sheets) is used to style HTML elements
- It controls layout, colors, fonts, spacing, and responsiveness

## ✅ Why CSS?
- Separates content (HTML) from design
- Reusable styles
- Enables responsive layouts for all devices

---

## 🗂️ CSS Folder Structure
Best practice:
```
project/
├── index.html
└── styles/
    └── style.css
```

---

## 🧪 3 Ways to Add CSS

### 1. Inline CSS
```html
<p style="color: red;">Hello</p>
```

### 2. Internal CSS
```html
<style>
  p { color: red; }
</style>
```

### 3. External CSS
```html
<link rel="stylesheet" href="styles/style.css">
```

---

## 💬 CSS Comments
```css
/* This is a comment */
```

---

## 🔍 Selectors

### Basic Selector
```css
p { color: red; }
```

### Grouped Selectors
```css
h1, h2, h3 { font-weight: bold; }
```

### Universal Selector
```css
* { margin: 0; padding: 0; }
```

### Class & ID Selectors
```css
.container { }  /* Class */
#main { }       /* ID */
```

---

## 🎨 Colors

### Named Colors
```css
color: red;
```

### RGB & RGBA Colors
```css
color: rgba(255, 0, 0, 0.5);
```

### HEX Colors
```css
color: #ff0000;
```

### HSL & HSLA Colors
```css
color: hsla(0, 100%, 50%, 0.5);
```

---

## 🖼️ Background
```css
background-color: lightblue;
background-image: url("bg.png");
background-size: cover;
background-repeat: no-repeat;
```

---

## 🧱 Borders
```css
border: 2px solid black;
border-radius: 10px;
```

---

## 📦 Box Model
Components:
- **Margin**: outer space
- **Border**: edge
- **Padding**: inner space
- **Content**: the actual content

```css
box-sizing: border-box;
```

---

## ➖ Margin / Padding / Outline
```css
margin: 10px;
padding: 20px;
outline: 2px dotted red;
```

---

## ✍️ Text Properties
```css
text-align: center;
text-decoration: underline;
text-transform: uppercase;
vertical-align: middle;
```

---

## ✨ Text Effects
```css
text-shadow: 2px 2px 5px gray;
```

---

## 🔠 Fonts
```css
font-family: 'Poppins', sans-serif;
font-size: 16px;
font-weight: bold;
```

---

## 🔗 Links
```css
a:link, a:visited, a:hover, a:active {
  color: blue;
}
```

---

## 📃 Lists
```css
ul {
  list-style-type: square;
}
```

---

## 📐 Block vs Inline
- **block**: takes full width
- **inline**: takes only as much width as needed

```css
display: block;
display: inline;
```

---

## 🔲 Display Property
```css
display: block;
display: inline;
display: flex;
display: none;
```

---

## 📏 Box Sizing
```css
box-sizing: border-box;
```

---

## 🧭 Flexbox Basics
```css
display: flex;
justify-content: center;
align-items: center;
flex-direction: row;
```

---

## 📱 Media Queries
```css
@media (max-width: 768px) {
  body { background-color: lightgray; }
}
```

---

## 🔁 Transform
```css
transform: rotate(10deg);
transform: scale(1.2);
```

---

## 📁 Mini-Project: Profile Card

A simple profile card using Flexbox and text effects:

### index.html
```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Profile Card</title>
  <link rel="stylesheet" href="style.css">
</head>
<body>
  <div class="card">
    <img src="https://via.placeholder.com/100" alt="Profile">
    <h2>Manas Kolaskar</h2>
    <p>Full-Stack Developer</p>
    <a href="#">GitHub</a>
  </div>
</body>
</html>
```

### style.css
```css
body {
  display: flex;
  justify-content: center;
  align-items: center;
  height: 100vh;
  background: linear-gradient(to right, #4e54c8, #8f94fb);
  font-family: 'Arial', sans-serif;
}

.card {
  background: white;
  padding: 30px;
  text-align: center;
  border-radius: 10px;
  box-shadow: 0 10px 20px rgba(0,0,0,0.2);
}

.card img {
  border-radius: 50%;
}

.card a {
  text-decoration: none;
  color: #4e54c8;
}
```
