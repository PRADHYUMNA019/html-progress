# Day 5 HTML - Table Attributes and Customization

## Overview
This HTML document demonstrates **various table formatting techniques** using HTML attributes and inline CSS styles.  
It covers row width, column width, row height, and using vertical headers.

---

## HTML Features Demonstrated

### 1. **Table with Row Width**
```html
<table border="1">
    <tr style="width:70%;">
        <th>Firstname</th>
        <th>Lastname</th>
        <th>City</th>
    </tr>
    <tr>
        <td>Eve</td>
        <td>Jackson</td>
        <td>New York</td>
    </tr>
    <tr>
        <td>John</td>
        <td>Doe</td>
        <td>Los Angeles</td>
    </tr>
</table>
```
**Explanation:**
- The `<tr>` tag has a `style="width:70%;"` property to set **row width**.
- **Border attribute** (`border="1"`) creates visible table borders.

---

### 2. **Table with Column Width**
```html
<table style="border:2px solid blue;">
    <tr>
        <th style="width:70%;">Student Name</th>
        <th style="width:70%">Age</th>
        <th style="width:70%">Percentage</th>
    </tr>
    <tr>
        <td align="center">Nina</td>
        <td align="center">20</td>
        <td align="center">85%</td>
    </tr>
    <tr>
        <td align="center">Raju</td>
        <td align="center">22</td>
        <td align="center">90%</td>
    </tr>
</table>
```
**Explanation:**
- Individual `<th>` elements use `style="width:70%;"` to control **column width**.
- `align="center"` centers the text within cells.
- The table has a **blue border** defined via `style`.

---

### 3. **Table with Row Height**
```html
<table style="border: 2px inset orange;">
    <tr>
        <th>Firstname</th>
        <th>Lastname</th>
        <th>Age</th>
    </tr>
    <tr height="100px;">
        <td>Raju</td>
        <td>XYZ</td>
        <td>20</td>
    </tr>
    <tr>
        <td>Mahesh</td>
        <td>ABC</td>
        <td>25</td>
    </tr>
</table>
```
**Explanation:**
- The `<tr>` has `height="100px;"` to set row height.
- Table border style is `inset` with orange color.

---

### 4. **Vertical Headers / First Column as Header**
```html
<table border="1">
    <tr>
        <th>Firstname</th>
        <th>Jill</th>
        <th>Eve</th>
    </tr>
    <tr>
        <th>Lastname</th>
        <td>Michael</td>
        <td>Jackson</td>
    </tr>
    <tr>
        <th>Age</th>
        <td>30</td>
        <td>26</td>
    </tr>    
</table>
```
**Explanation:**
- The **first column** uses `<th>` tags instead of `<td>`, making them **vertical headers**.
- This approach helps highlight row titles while keeping other cells as normal data.

---

## Key Takeaways
- **Row Width:** Can be set via inline CSS on `<tr>`.
- **Column Width:** Can be set individually via inline CSS on `<th>` or `<td>`.
- **Row Height:** Can be adjusted via the `height` attribute or CSS styling.
- **Vertical Headers:** Use `<th>` in the first column to represent row titles.

---

## Output Preview
When opened in a browser:
1. The first table has a **wide header row**.
2. The second table has **wide columns** and centered content.
3. The third table has a **tall row** due to height styling.
4. The last table has **vertical headers** for rows.

---

## How to Run
1. Save the HTML code as `day5.html`.
2. Open the file in any web browser.
3. Observe the different table styling techniques in action.

---

**Date:*11 th april 2025* Day 5 of HTML Learning
