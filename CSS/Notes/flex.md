# CSS Flexbox

Flexbox (Flexible Box Layout) is a CSS layout model used to arrange, align, and distribute elements inside a container.

To use Flexbox, set the parent element's `display` property to `flex`.

### Example

```css
.container{
    display: flex;
}
```

All direct child elements become **flex items**.

---

# 1. `display: flex`

* Makes an element a **flex container**.
* All direct child elements become **flex items**.

### Example

```css
.container{
    display: flex;
}
```

---

# 2. `flex-direction`

* Defines the direction in which flex items are arranged.

### Values

* `row` (default)
* `row-reverse`
* `column`
* `column-reverse`

### Example

```css
.container{
    display: flex;
    flex-direction: row;
}
```

### Explanation

* `row` → Items are arranged from left to right.
* `column` → Items are arranged from top to bottom.

---

# 3. `justify-content`

* Aligns items along the **main axis** (horizontal when `flex-direction: row`).

### Values

* `flex-start`
* `center`
* `flex-end`
* `space-between`
* `space-around`
* `space-evenly`

### Example

```css
.container{
    display: flex;
    justify-content: center;
}
```

### Explanation

`justify-content: center;` places all flex items at the center of the container.

---

# 4. `align-items`

* Aligns items along the **cross axis** (vertical when `flex-direction: row`).

### Values

* `stretch`
* `flex-start`
* `center`
* `flex-end`

### Example

```css
.container{
    display: flex;
    align-items: center;
}
```

### Explanation

`align-items: center;` vertically centers all flex items inside the container.

---

# 5. `gap`

* Adds space between flex items.

### Example

```css
.container{
    display: flex;
    gap: 20px;
}
```

### Explanation

A `20px` gap is added between each flex item.

---

# 6. `flex-wrap`

* Determines whether flex items move to the next line when there is not enough space.

### Values

* `nowrap` (default)
* `wrap`
* `wrap-reverse`

### Example

```css
.container{
    display: flex;
    flex-wrap: wrap;
}
```

### Explanation

When there is not enough space in the container, the flex items automatically move to the next line.

---

# Example

```css
.gallery{
    display: flex;
    flex-direction: row;
    justify-content: center;
    align-items: center;
    gap: 30px;
    flex-wrap: wrap;
}
```

### Explanation

* `display: flex;` → Makes `.gallery` a flex container.
* `flex-direction: row;` → Arranges images from left to right.
* `justify-content: center;` → Centers the images horizontally.
* `align-items: center;` → Centers the images vertically.
* `gap: 30px;` → Adds 30px spacing between images.
* `flex-wrap: wrap;` → Moves images to the next line if there isn't enough space.

---

# Important Note

* **display: flex** → Turns the container into a flex container.
* **flex-direction** → Controls the direction of flex items.
* **justify-content** → Aligns items along the main axis.
* **align-items** → Aligns items along the cross axis.
* **gap** → Adds space between flex items.
* **flex-wrap** → Allows items to move to the next line when needed.
