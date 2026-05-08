# VerbaNexAI Lab Website

![HTML5](https://img.shields.io/badge/html5-%23E34F26.svg?style=for-the-badge&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/css3-%231572B6.svg?style=for-the-badge&logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/javascript-%23323330.svg?style=for-the-badge&logo=javascript&logoColor=%23F7DF1E)
![Bootstrap](https://img.shields.io/badge/bootstrap-%238511FA.svg?style=for-the-badge&logo=bootstrap&logoColor=white)

This repository contains the source code for the official website of the **VerbaNexAI Lab**, a research group at the Universidad Tecnológica de Bolívar (UTB), Cartagena, Colombia. 

The lab focuses on cutting-edge research in Artificial Intelligence, Natural Language Processing (NLP), Computer Vision, and Predictive Analytics.

🌐 **Live Website:** [https://verbanexai.github.io/](https://verbanexai.github.io/)

---

## 🎨 Design Features

The website was recently redesigned to reflect a modern, academic, and technological aesthetic:
- **Glassmorphism UI:** Semi-transparent cards with blurred backgrounds.
- **Interactive Background:** A neural network particle effect powered by `particles.js`.
- **Dark / Light Mode:** Native support with a toggle button that saves user preferences via `localStorage`.
- **Fluid Navigation:** Smooth fade-in/fade-out page transitions.
- **Scroll Animations:** Integrated with `AOS.js` for dynamic content revealing.
- **Fully Responsive:** Built on top of Bootstrap 5.

## 📂 Repository Structure

To maintain clean URLs (e.g., `/publications/` instead of `/publications.html`), the repository is structured using subdirectories containing `index.html` files.

```text
verbanexai.github.io/
│
├── index.html               # Home Page
│
├── publications/
│   └── index.html           # Publications timeline and filtering
│
├── projects/
│   └── index.html           # Lab initiatives and Master's thesis projects
│
├── teaching/
│   └── index.html           # Academic courses and seminars
│
├── repositories/
│   └── index.html           # Links to open-source GitHub repos
│
├── people/
│   └── index.html           # Lab researchers and staff directory
│
└── blog/
    ├── index.html           # Blog posts list
    └── your-post/
        └── index.html       # Individual blog post template
```

## 🛠️ How to Add Content

Because this site uses pure HTML/JS without a static site generator in this branch, follow these guidelines to update content:

### Adding a New Person (People Section)
Edit `people/index.html` and add a new block inside the corresponding row (`<div class="row g-4">`):
```html
<div class="col-lg-4 col-md-6" data-aos="fade-up">
    <div class="card h-100 pub-card person-card">
        <div class="person-img-container">
            <img src="URL_TO_IMAGE" alt="Name" class="person-img">
        </div>
        <h3 class="person-name">Name</h3>
        <p class="person-title">Role / Title</p>
        <p class="person-bio">Short biography...</p>
    </div>
</div>
```

### Adding a New Blog Post
1. Create a new folder inside `/blog/` (e.g., `/blog/my-new-paper/`).
2. Create an `index.html` file inside that folder.
3. Copy the HTML from an existing blog post and replace the text.
4. Update the main list in `/blog/index.html` to link to your new folder: `href="/blog/my-new-paper/"`.

## 🚀 Deployment

This website is hosted using **GitHub Pages**. 
To deploy changes:
1. Make your edits in your local repository.
2. Commit and push the changes to the specific deployment branch (e.g., `verbanex_gh` or `labpage`).
3. GitHub Actions will automatically rebuild and deploy the site within 1-3 minutes.

## 🔬 About VerbaNexAI Lab

Located at the *School of Digital Transformation, Parque Industrial y Tecnológico Carlos Vélez Pombo Km 1 Vía Turbaco, Cartagena de Indias, Colombia*. 

We generate actionable insights for automated inspection, efficient energy management, and adaptive learning environments, all within an open collaboration and reproducible research framework.

---
*Maintained by the VerbaNexAI Lab Team.*
