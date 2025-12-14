## 📌 GitHub Pages: Static Hosting Only
GitHub Pages is a static site hosting service.
It does not run backend code or servers.

### What “static” means:
* Files are served as-is from a CDN
* No server-side execution (no Node.js, Python, Java, etc.)
* No databases or APIs hosted on GitHub Pages

## 🚀 GitHub Pages Deployment (Behind the Scenes)

This project is hosted using **GitHub Pages**.

When GitHub Pages is enabled (**Settings → Pages → main branch → root**), GitHub automatically sets up a **system-managed GitHub Actions workflow** called:

```
pages-build-deployment
```

This workflow is created and maintained by GitHub. No manual CI/CD configuration or YAML files are required.

---

## 🔧 What Happens Automatically

* Every push to the `main` branch triggers deployment
* GitHub checks out the repository
* Detects the site type (static in this case)
* Skips build steps (no Jekyll / Node / npm)
* Publishes files as a Pages artifact
* Deploys the site to a CDN-backed GitHub Pages server

The website is **not served directly from the repository**, but from the deployed artifact.

---
## 🌐 Hosting & Accessibility

This website is hosted using **GitHub Pages** and is **publicly accessible** by default.

* **Live URL:** `https://username.github.io`
* **Access:** Public (no authentication required)
* **Hosting:** GitHub Pages (CDN-backed)
* **Protocol:** HTTPS enabled

The site is served from GitHub’s global CDN, not directly from the repository, ensuring fast and reliable access worldwide.

---

## 🔎 Why It Is Public

* GitHub Pages sites are public by default
* Content is served via CDN endpoints
* Anyone with the URL can access the website
* Repository visibility controls source access, not website access

> ⚠️ Note: Even if the repository is private (GitHub Pro/Enterprise), GitHub Pages can still expose the site publicly unless explicitly restricted.

---

## 🔄 Deployment Flow

```text
Content Update
(Code / Static Files)
        ↓
Source Repository
(GitHub Repository)
        ↓
GitHub Pages Enabled
(Repository Settings)
        ↓
Pages Build & Deploy Workflow
(GitHub-managed Action)
        ↓
Site Processing
• Detect site type (static / Jekyll)
• Optional build step
        ↓
Pages Artifact Creation
(Prepared website files)
        ↓
Deployment to Pages Environment
(github-pages)
        ↓
GitHub Pages Infrastructure
(Global CDN)
        ↓
Live Website
(<username>.github.io or custom domain)
```

---

## ✅ Key Benefits

* Zero configuration CI/CD
* Automatic redeploy on every change
* CDN-backed performance
* Versioned deployments & rollbacks
* Enterprise-grade pipeline, simplified

Absolutely — here’s a **short, clean, README-ready note** you can paste directly 👇

---

## 📄 GitHub Pages Support

**GitHub Pages is a static site hosting service.**

### ✅ Supported

* Static files: **HTML, CSS, JavaScript**
* Assets: images, fonts, JSON
* Frontend frameworks (**React, Vue, Angular, etc.**) - After build [compile → bundle → output static files]
* UI libraries (Tailwind, Material UI, Bootstrap)
* GitHub Actions–based build & deploy workflows

### ❌ Not Supported

* Backend/server-side code (Node.js, Python, Java, etc.)
* Server-Side Rendering (SSR)
* Databases or APIs

> **Rule of thumb:** If your app can be built into static files, GitHub Pages can host it.

---

