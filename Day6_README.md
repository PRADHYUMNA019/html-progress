# 📅 Day 6 – HTML Tables: Cell Padding & Border Spacing

## 📌 Overview
This HTML document demonstrates the difference between **cell padding** and **border spacing** in HTML tables.  
It contains two sections:
1. **Table with Cell Padding** – Controls space *inside* the table cells.
2. **Table with Border Spacing** – Controls space *between* the table cells.

---

## 🖥 Code Explanation

### 1️⃣ Table with Cell Padding
```html
<table>
    <tr>
        <th>Firstname</th>
        <th>Lastname</th>
        <th>Marks</th>
    </tr>
    <tr>
        <td>John</td>
        <td>Doe</td>
        <td>85</td>
    </tr>
    <tr>
        <td>Jane</td>
        <td>Smith</td>
        <td>90</td>
    </tr>
</table>
```
- Uses **default table styling**.
- Padding here is controlled by the browser default or manually via the `padding` property inside `th` or `td` tags.
- This example uses `border-spacing: 10px;` in the CSS, but since the border is collapsed, only cell padding is visually noticed.

---

### 2️⃣ Table with Border Spacing
```html
<table style="border: 2px solid green; border-spacing: 15px; border-collapse: separate;">
    <tr>
        <th style="padding: 20px;">Product</th>
        <th style="padding: 20px;">Price</th>
    </tr>
    <tr>
        <td style="padding: 20px;">Laptop</td>
        <td style="padding: 20px;">1000</td>
    </tr>
    <tr>
        <td style="padding: 20px;">Smartphone</td>
        <td style="padding: 20px;">500</td>
    </tr>
</table>
```
- `border-collapse: separate;` ensures cells have **separate borders**, allowing `border-spacing` to work.
- `border-spacing: 15px;` adds **15px gap between cells**.
- `padding: 20px;` ensures there is space **inside** each cell.

---

## 🎯 Key Concepts

| Property/Attribute | Purpose | Applies To |
|--------------------|---------|------------|
| `padding`          | Space **inside** a cell between content and border | Table cells (`td`, `th`) |
| `border-spacing`   | Space **between** table cells | The table element |
| `border-collapse`  | Controls whether borders are **shared** (`collapse`) or **separate** (`separate`) | The table element |

---

## 📷 Visual Difference

- **Cell Padding** → Space *inside* the cell content area.
- **Border Spacing** → Space *between* the outer edges of cells.

---

## 🏁 Final Output Screenshot (Conceptual)

**Table with Cell Padding**
```
+-----------+-----------+-------+
|  John     |   Doe     |  85   |
+-----------+-----------+-------+
```

**Table with Border Spacing**
```
+-----------+           +-----------+
|  Laptop   |           |  1000     |
+-----------+           +-----------+
```

---

## 📄 Full HTML Code
```html
<html>
    <head>
        <title>Day 6</title>
        <style>
            table {
                border-collapse: separate;
                border-spacing: 10px;
            }
        </style>
    </head>
    <body>
        <h3>Table with cell padding</h3>
        <table>
            <tr>
                <th>Firstname</th>
                <th>Lastname</th>
                <th>Marks</th>
            </tr>
            <tr>
                <td>John</td>
                <td>Doe</td>
                <td>85</td>
            </tr>
            <tr>
                <td>Jane</td>
                <td>Smith</td>
                <td>90</td>
            </tr>
        </table>
        <br><br>
        <h3>Table with border spacing</h3>
        <table style="border: 2px solid green; border-spacing: 15px; border-collapse: separate;">
            <tr>
                <th style="padding: 20px;">Product</th>
                <th style="padding: 20px;">Price</th>
            </tr>
            <tr>
                <td style="padding: 20px;">Laptop</td>
                <td style="padding: 20px;">1000</td>
            </tr>
            <tr>
                <td style="padding: 20px;">Smartphone</td>
                <td style="padding: 20px;">500</td>
            </tr>
        </table>
    </body>
</html>
```

---

✅ **Tip**: Always use CSS instead of old HTML attributes (`cellpadding`, `cellspacing`) for modern, maintainable code.
