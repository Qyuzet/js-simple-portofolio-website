# JS Simple Portfolio Website

## Overview

The **JS Simple Portfolio Website** project is a basic portfolio template designed to showcase your work and personal information. This website focuses on demonstrating dark and light mode features.
[TRY NOW!](https://qyuzet.github.io/js-simple-portofolio-website/)


![image](https://github.com/Qyuzet/js-simple-portofolio-website/assets/93258081/84264203-e591-4479-a550-1405cd3e19f8)

![image](https://github.com/Qyuzet/js-simple-portofolio-website/assets/93258081/df42b577-999c-433f-b947-436ae42bde3b)


## Features

- **Dark and Light Mode**: Toggle between dark and light themes.
- **Personal Information Section**: Brief introduction about yourself.
- **Project Showcase**: Display your projects with descriptions and links.
- **Contact Information**: Easy-to-find contact details.

## Installation

1. Clone the repository:
    ```bash
    git clone https://github.com/Qyuzet/js-simple-portofolio-website.git
    ```
2. Navigate to the project directory:
    ```bash
    cd js-simple-portofolio-website
    ```
3. Open `index.html` in your web browser.

## File Structure

- **index.html**: Main HTML file.
- **style.css**: Styling file.
- **scripts.js**: JavaScript file for functionality.

## Usage

To toggle between dark and light modes, click the button provided on the website. This will change the theme accordingly. 

## Code Explanation

Here's the updated README for your GitHub repository:

---

# JS Simple Portfolio Website

This project is a simple portfolio website focused on showcasing the dark and light mode feature. The web is not responsive yet.

## Demo

[Live Demo](https://your-demo-link.com)

## Features

- **Dark/Light Mode Toggle**: Easily switch between dark and light themes.
- **Local Storage**: Remembers the user's theme preference.

## Code Explanation

### Theme Initialization

```javascript
var icon = document.getElementById("icon");

if (localStorage.getItem("theme") == null) {
  localStorage.setItem("theme", "light");
}
```
- Retrieves the theme icon element.
- Sets the default theme to "light" if not already set.

### Applying Saved Theme

```javascript
let localData = localStorage.getItem("theme");

if (localData == "light") {
  icon.src = "images/moon.png";
  document.body.classList.remove("dark-theme");
} else if (localData == "dark") {
  icon.src = "images/sun.png";
  document.body.classList.add("dark-theme");
}
```
- Retrieves and applies the saved theme.
- Updates the theme icon and body class accordingly.

### Theme Toggle Function

```javascript
icon.onclick = function () {
  document.body.classList.toggle("dark-theme");
  if (document.body.classList.contains("dark-theme")) {
    icon.src = "images/sun.png";
    localStorage.setItem("theme", "dark");
  } else {
    icon.src = "images/moon.png";
    localStorage.setItem("theme", "light");
  }
};
```
- Toggles between dark and light themes on icon click.
- Updates the icon and saves the current theme in local storage.


## Demo

Check out the live demo [here](https://qyuzet.github.io/js-simple-portofolio-website/).

## Contributing

Feel free to fork this repository and make changes. Contributions are welcome!

## License

This project is licensed under the MIT License.
