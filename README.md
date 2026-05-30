# 🎀 Birthday Website for XYZ

A beautifully crafted Apple-inspired birthday website featuring smooth scroll animations, elegant pink aesthetics, password protection, and immersive reveal effects designed to create a memorable birthday experience.

## 🌐 Live Demo

<p align="center">
  <a href="https://moin-shadab.github.io/girlfriend-friend-birthday-wish/" target="_blank">
    View Live Website →
  </a>
</p>

---

## ✨ Features

* Apple-style scroll storytelling experience
* Password-protected entry screen
* Smooth animations and scroll-triggered reveals
* Customizable photo galleries and memories
* Personalized messages, pickup lines, and special moments
* Responsive design for desktop and mobile devices
* No external dependencies required

---

## 🛠 Customization Guide

Open the `index.html` file and locate the `CONFIG` object near the beginning of the `<script>` section.

```javascript
const CONFIG = {
  name: "XYZ",
  password: "1430",

  pinSlides: [
    {
      img: "images/photo1.jpg",
      heading: "Her Smile",
      body: "..."
    }
  ],

  pickupLines: [ ... ],
  reasons: [ ... ],
  memories: [ ... ]
};
```

### Personalize the Website

| Setting       | Description                                       |
| ------------- | ------------------------------------------------- |
| `name`        | Display name shown throughout the website         |
| `password`    | Secret code required to unlock the experience     |
| `pinSlides`   | Featured storytelling slides with images and text |
| `pickupLines` | Cute and romantic messages                        |
| `reasons`     | Reasons why she is special                        |
| `memories`    | Photo gallery and memorable moments               |

---

## 🖼 Adding Photos

### Option 1: Store Images in the Repository (Recommended)

1. Create an `images/` folder in the project root.
2. Upload your photos to the folder.
3. Reference them inside the configuration.

Example:

```javascript
img: "images/photo1.jpg"
```

---

### Option 2: Use External Image URLs

Upload images to a hosting service such as Imgur or Google Drive and use the direct image URL.

Example:

```javascript
img: "https://i.imgur.com/example.jpg"
```

---

## 📌 Where Images Are Used

| Configuration Key       | Purpose                                        |
| ----------------------- | ---------------------------------------------- |
| `pinSlides[i].img`      | Main Apple-style storytelling sections         |
| `memories[i].img`       | Memory gallery and photo wall                  |
| HTML image placeholders | Additional reveal sections throughout the page |

For custom reveal sections, replace the existing placeholder elements with:

```html
<img src="your-image-url.jpg" alt="Memory">
```

---

## 🎨 Customizing Colors

The website uses CSS variables for easy theme customization. Edit the values inside the `:root` selector:

```css
--pink-deep:  #c9517a;
--pink-main:  #e8789a;
--pink-soft:  #f4a7be;
--pink-blush: #fce4ec;
```

Feel free to replace these colors with any palette that matches your preferred style.

---

## 🔒 Password Protection

The default password is:

```javascript
password: "1430"
```

Simply replace it with your preferred code.

Additional effects include:

* Animated heart-style password masking
* Visual feedback for incorrect entries
* Smooth unlock animation upon successful authentication

---

## 🚀 Deployment

This project is designed to work seamlessly with GitHub Pages.

1. Push the repository to GitHub.
2. Open **Settings → Pages**.
3. Select the deployment branch.
4. Save the configuration.
5. Your birthday website will be live within a few moments.

---

## 💗 Author

Created by **Moin Shadab**

A lightweight, single-file project built to be easy to customize, easy to deploy, and memorable for someone special.
