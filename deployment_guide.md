# Deployment Guide: Educational Management Suite

This project is a collection of high-fidelity static HTML files. To deploy it and make it accessible via a public URL, you can use any of the following modern hosting platforms.

## Option 1: Vercel (Recommended - Fastest)
Vercel is perfect for static sites. It's fast, free for personal use, and provides automatic SSL.

1.  **Visit [Vercel](https://vercel.com/new)**.
2.  **Drag and Drop**: Simply drag the entire `combine` folder onto the "Deploy" area.
3.  **Wait**: Vercel will process the files and provide you with a production URL (e.g., `educational-suite.vercel.app`).
4.  **Entry Point**: Your `index.html` (which I've created) will automatically serve as the homepage.

---

## Option 2: Netlify (Alternative)
Netlify is another excellent choice with a similar "drag-and-drop" experience.

1.  **Visit [Netlify Drop](https://app.netlify.com/drop)**.
2.  **Upload**: Drag the `combine` folder into the dotted box.
3.  **Deploy**: Once uploaded, your site is live instantly.
4.  **Customization**: You can rename the generated URL in the site settings.

---

## Option 3: GitHub Pages (Best for Version Control)
If you want to keep your code in a repository and have it update automatically:

1.  **Initialize Git** (if not already done):
    ```bash
    git init
    git add .
    git commit -m "Initial commit"
    ```
2.  **Push to GitHub**: Create a new repository on GitHub and push your code there.
3.  **Enable Pages**:
    *   Go to your repository **Settings**.
    *   Click on **Pages** in the left sidebar.
    *   Under "Build and deployment", select the `main` branch and `/ (root)` folder.
    *   Click **Save**.
4.  **Live Site**: Your site will be available at `https://USERNAME.github.io/REPO_NAME/`.

---

## Local Preview
To test the site locally as it would appear on a server, you can use a simple node server:

```bash
npx serve .
```

This will host the site at `http://localhost:3000`.
