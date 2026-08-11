# Big Portfolio — Debugged Version

A responsive personal portfolio website built with **HTML, CSS and JavaScript**. This repository contains the cleaned and debugged version of the original project.

## ✨ Features

- Responsive portfolio layout
- Sticky navigation bar
- Mobile navigation menu
- Dark/light mode toggle
- Animated profession section
- ScrollReveal animations
- Swiper testimonial slider
- Services section
- Portfolio gallery
- Contact form UI
- Responsive breakpoints for mobile, tablet and desktop

## 🛠️ Tech Stack

- HTML5
- CSS3
- JavaScript
- [Swiper](https://swiperjs.com/)
- [ScrollReveal](https://scrollrevealjs.org/)
- [Boxicons](https://boxicons.com/)
- Google Fonts — Poppins

## 📁 Project Structure

```text
big-portfolio/
├── index.html
├── style-1.css
├── script-1.js
├── images/
│   ├── PNG/
│   │   ├── ravi img (4).png
│   │   ├── rr.png
│   │   └── Untitled design.png
│   └── Web Images/
│       ├── web1.jpg
│       ├── web2.jpg
│       ├── web3.jpeg
│       ├── web4.jpg
│       ├── web6.jpg
│       ├── web7.jpg
│       ├── web8.jpg
│       ├── web9.jpg
│       └── testimonial/project images
└── README.md
```

## 🐛 Debugging Performed

The original project was checked for broken asset paths, JavaScript issues and obvious HTML/CSS problems.

### Fixed

1. **Broken image paths**
   - The HTML referenced images directly inside `images/`.
   - The actual files were stored inside `images/PNG/` and `images/Web Images/`.
   - All affected references were corrected.

2. **Broken testimonial image paths**
   - Testimonial images were referenced from the project root.
   - They were actually stored in `images/Web Images/`.
   - References were corrected.

3. **CSS typo**
   - Fixed:
     ```css
     padding: 3rem 2ren 4rem;
     ```
   - To:
     ```css
     padding: 3rem 2rem 4rem;
     ```

4. **Duplicate Swiper JavaScript**
   - Swiper JavaScript was loaded in the `<head>` and again at the bottom.
   - The duplicate load was removed.

5. **JavaScript selector safety**
   - Navigation and dark-mode handlers now check whether required elements exist before using them.
   - Active navigation selection was made more reliable.

6. **Contact form input types**
   - Mobile number changed from `number` to `tel`.
   - Email Subject changed from `email` to `text`.

7. **GitHub Pages entry file**
   - Renamed `index-1.html` to `index.html` so GitHub Pages can use it as the default entry point.

8. **macOS metadata cleanup**
   - `.DS_Store` and extracted macOS metadata were removed from the final project package.

## ⚠️ Important Remaining Items

These are not code bugs but should be completed before using the portfolio as a real production website:

### 1. Placeholder content

The website still contains Lorem Ipsum text. Replace it with real:

- About information
- Service descriptions
- Project descriptions
- Testimonials

### 2. Placeholder links

Several buttons and social links currently use:

```html
href="#"
```

Replace them with real URLs or section links.

### 3. Contact form backend

The contact form currently has no backend/email service attached. Submitting the form will not automatically send the message anywhere.

You can later connect it to a form service or your own backend/API.

### 4. Download CV

The `Download CV` button needs a real CV/PDF file and download link.

### 5. Portfolio project links

Each portfolio project's external-link button should point to its actual live project or case study.

## 🚀 Run Locally

Because this is a static website, you can open `index.html` directly in a browser.

For a better development workflow, use VS Code with a local server such as Live Server.

## 🌐 Deploy on GitHub Pages

1. Create a new GitHub repository.
2. Upload all files from this project.
3. Make sure `index.html` is in the repository root.
4. Open **Settings → Pages**.
5. Select the deployment source/branch.
6. Save the settings.
7. GitHub Pages will provide the public website URL.

## 📱 Responsive Testing

Test the website at minimum at:

- 1440px desktop
- 1024px tablet/desktop
- 768px tablet
- 617px mobile
- 450px mobile
- 365px small mobile

## 🔒 Security Notes

Do not commit:

- API keys
- Passwords
- Private tokens
- `.env` files containing secrets
- Database credentials

## 📌 Project Status

**Status: Debugged / Demo Ready**

The major broken local asset references and obvious JavaScript/CSS issues found in the supplied project have been corrected.

Production readiness still requires replacing placeholder content and connecting the contact/project links.

## 👨‍💻 Author

**Ravi Menariya**

Personal portfolio project.

---

⭐ If you like the project, consider giving the repository a star.
