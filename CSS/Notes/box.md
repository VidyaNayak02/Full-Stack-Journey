# CSS Box Model

Every HTML element is treated as a **box**. The CSS Box Model describes how the size and spacing of an element are calculated.

The Box Model consists of **four parts**:

1. Content
2. Padding
3. Border
4. Margin

---

# Box Structure

```text
+-----------------------------------------+
|               Margin                    |
|  +-----------------------------------+  |
|  |              Border               |  |
|  |  +-----------------------------+  |  |
|  |  |          Padding            |  |  |
|  |  |  +-----------------------+  |  |  |
|  |  |  |      Content          |  |  |  |
|  |  |  +-----------------------+  |  |  |
|  |  +-----------------------------+  |  |
|  +-----------------------------------+  |
+-----------------------------------------+
```

---

# 1. Content

* The actual content of an element.
* It can contain text, images, buttons, etc.
* The `width` and `height` properties apply to the content area by default.

### Example

```css
.box{
    width: 300px;
    height: 150px;
}
```

---

# 2. Padding

* Space between the **content** and the **border**.
* Increases the size of the element.
* The background color extends into the padding.

### Example

```css
.box{
    padding: 20px;
}
```

---

# 3. Border

* A line surrounding the padding and content.
* Can have different widths, colors, and styles.

### Example

```css
.box{
    border: 2px solid black;
}
```

---

# 4. Margin

* Space outside the border.
* Creates distance between neighboring elements.
* The background color does **not** extend into the margin.

### Example

```css
.box{
    margin: 30px;
}
```

---

# Complete Example

```css
.box{
    width: 250px;
    height: 100px;
    padding: 20px;
    border: 3px solid blue;
    margin: 30px;
}
```

---

# Difference Between Padding and Margin

| Padding                     | Margin                          |
| --------------------------- | ------------------------------- |
| Space inside the border     | Space outside the border        |
| Background color is visible | Background color is not visible |
| Increases element size      | Creates space between elements  |

---

# Important Note

* **Content** → Actual text or image inside the element.
* **Padding** → Space between the content and the border.
* **Border** → Outline surrounding the element.
* **Margin** → Space outside the border between elements.
