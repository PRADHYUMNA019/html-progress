
# HTML Learning Project: Bookmarks, Images, Links, and Contact Section

This project demonstrates core HTML concepts in a single file, including bookmarks, images with attributes, styled anchor links, and a formatted contact section.

---

## 🧭 1. Bookmarks Navigation (Internal Page Links)

The page contains a **navigation bar** that allows smooth scrolling to different sections of the same page using internal bookmarks.

### ✅ Code Example:
```html
<nav>
  <a href="#home">Home</a>
  <a href="#about">About</a>
  <a href="#services">Services</a>
  <a href="#contact">Contact</a>
</nav>
```

Each section on the page includes an `id` to match the anchor links:

```html
<section id="home">
  <h1>Welcome to my website</h1>
  <a class="back-to-top" href="#top">Back to Top</a>
</section>
```

CSS is used to enable smooth scrolling and sticky navigation.

---

## 🖼️ 2. HTML Images and Attributes

The page demonstrates different ways to use the `<img>` tag in HTML.

### 🧱 Basic Image
```html
<img src="bgimg.jpg">
```

### 📷 With alt attribute (for accessibility and fallback)
```html
<img src="bgimg.jpg" alt="background image">
```

### 📐 With width and height
```html
<img src="bgimg.jpg" width="300" height="100">
```

### 💤 With loading attribute
```html
<img src="bgimg.jpg" loading="lazy">
<img src="bgimg.jpg" loading="eager">
```

### 📱 With `srcset` for responsiveness
```html
<img src="bgimg.jpg" 
     srcset="small.jpg 400w, medium.jpg 800w, large.jpg 1200w"
     alt="Beautiful landscape">
```

---

## 🗺️ 3. Image with Clickable Map (`usemap` and `<area>`)

The image contains clickable areas linking to external pages.

### ✅ Code Example:
```html
<img src="image.jpg" usemap="#my-map">
<map name="my-map">
  <area shape="rect" coords="..." href="..." alt="..." target="_blank">
</map>
```

Each `<area>` defines a region (rectangle or circle) on the image that can be clicked.

---

## 🎨 4. Background Image Using Inline CSS

Adds a background image to a paragraph using the `style` attribute.

### ✅ Example:
```html
<p style="background-image:url('image.jpg'); color:white;">
  This is a background image.
</p>
```

---

## 🔗 5. Anchor Link Styling with CSS Pseudo-Classes

Custom styles for different states of links using CSS:

### ✅ Styles Used:
```css
a:link    { color: green; }
a:visited { color: pink; }
a:hover   { color: red; text-decoration: underline; }
a:active  { color: yellow; text-decoration: underline; }
```

These styles change how links look when clicked, hovered, visited, or active.

---

## 📞 6. Contact Section with Semantic Formatting

A detailed contact section using semantic and formatting tags.

### ✅ Elements Used:
- `<strong>` for bold labels
- `<em>` for emphasized text
- `<a href="mailto:...">` for clickable email
- `<a href="tel:...">` for clickable phone
- `<address>` for structured location details

### 🧱 Example:
```html
<p><strong>Email:</strong> <a href="mailto:contact@example.com">contact@example.com</a></p>
<p><strong>Phone:</strong> <a href="tel:+1234567890">+1 (234) 567-890</a></p>
<address>
  123 Web Street,<br>
  Code City, CA 90210<br>
  United States
</address>
<p><em>We're available Monday to Friday, 9 AM to 6 PM.</em></p>
```

---

## ✅ Summary of Concepts Covered

| Feature               | Description |
|----------------------|-------------|
| `<img>`              | Various image formats and attributes |
| `srcset`             | Responsive images for different resolutions |
| `usemap` + `<area>`  | Clickable image areas |
| `nav` + bookmarks    | Internal navigation |
| `scroll-behavior`    | Smooth scrolling effect |
| `mailto:` / `tel:`   | Clickable contact links |
| Semantic tags        | `<strong>`, `<em>`, `<address>` |
| Link styling         | CSS pseudo-classes for anchor states |

---

This project serves as a beginner-friendly example of building a basic web page with HTML features used in real-world scenarios.
