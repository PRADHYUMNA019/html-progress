# Day 4 HTML - Tables

## Overview
This project demonstrates the usage of **HTML tables** with proper structure and styling.  
It contains two tables:

1. **Monthly Savings Table** – Displays month-wise savings data.
2. **Product Price Table** – Shows product names, prices, and total cost, using `<thead>`, `<tbody>`, and `<tfoot>`.

---

## HTML Features Used

### 1. `<table>`
Defines the table structure for tabular data.

### 2. `<caption>`
Provides a descriptive title for the table.

### 3. `<thead>`, `<tbody>`, `<tfoot>`
- `<thead>`: Groups table headers.
- `<tbody>`: Contains the main table content.
- `<tfoot>`: Displays the table footer (e.g., totals).

### 4. `<tr>`, `<th>`, `<td>`
- `<tr>`: Defines a table row.
- `<th>`: Table header cell (bold & centered by default).
- `<td>`: Table data cell.

### 5. CSS Styling
The table uses inline CSS in the `<style>` tag:
```css
table, th, td {
    border-collapse: collapse;
    border: 1px solid black;
    padding: 5px;
    background-color: lightsteelblue;
}
```

**CSS properties explained:**
- **border-collapse: collapse;** → Merges table borders into a single border.
- **border: 1px solid black;** → Adds a solid black border to cells.
- **padding: 5px;** → Adds spacing between cell content and borders.
- **background-color: lightsteelblue;** → Sets a soft blue background.

---

## Code Breakdown

### Monthly Savings Table
```html
<table border="1">
    <caption>Monthly savings</caption>
    <tr>
        <th>Month</th>
        <th>Savings</th>
    </tr>
    <tr>
        <td>January</td>
        <td>100 bucks</td>
    </tr>
    <tr>
        <td>February</td>
        <td>50 bucks</td>
    </tr>
</table>
```

### Product Price Table
```html
<table border="1">
  <thead>
    <tr>
      <th>Product</th><th>Price</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>Laptop</td><td>$1000</td>
    </tr>
    <tr>
      <td>Mouse</td><td>$20</td>
    </tr>
  </tbody>
  <tfoot>
    <tr>
      <td>Total</td><td>$1020</td>
    </tr>
  </tfoot>
</table>
```

---

## Key Takeaways
- `<thead>`, `<tbody>`, and `<tfoot>` improve table readability and accessibility.
- CSS styling enhances the appearance of tables.
- `<caption>` adds context to the data presented

