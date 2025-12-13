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

## 🌐 Hosting Details

* Live URL: `https://username.github.io`
* Served via **global CDN**
* HTTPS enabled by default
* Fast, scalable, production-grade hosting

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
