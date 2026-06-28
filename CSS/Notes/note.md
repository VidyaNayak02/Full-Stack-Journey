# CSS Selectors

CSS selectors are used to select HTML elements and apply styles to them.

---

# 1. Element Selector

* Selects **all elements** of the same HTML tag.
* No special symbol is used.

### Examples

```css
h1{
    color: blue;
}

body{
    background-image: url("");
}

p{
    color: white;
}
```

### Explanation

* The blue color is applied to **all `<h1>` elements**, no matter how many are present in the HTML file.
* The background image is applied to the **entire `<body>`** of the webpage.
* The white text color is applied to **all `<p>` elements**.

---

# 2. Class Selector (`.`)

* Selects **multiple elements** with the same class name.
* Starts with a **dot (`.`)**.
* Can be reused on multiple elements.

### Syntax

```css
.modify{
    color: red;
}
```

```html
<h1 class="modify">Heading</h1>
<p class="modify">Paragraph</p>
```

### Explanation

Both the `<h1>` and `<p>` elements with the class **modify** will have red text. Other elements remain unchanged.

---

# 3. ID Selector (`#`)

* Selects **one unique element**.
* Starts with a **hash (`#`)**.
* Should be used only once per webpage.

### Syntax

```css
#title{
    color: green;
}
```

```html
<h1 id="title">Welcome</h1>
```

### Note

ID selectors can also be used with anchor links (`<a href="#title">`) to navigate to a specific section of the webpage.

---

# Important Note

* **Element Selector** (No symbol) → Styles all elements of a specific HTML tag.
* **Class Selector (`.`)** → Styles multiple elements having the same class name.
* **ID Selector (`#`)** → Styles one unique element.
