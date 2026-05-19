## 🛠️ How This Project Was Built and Deployed

This project is a React-based Single Page Application (SPA) built with **Vite** and deployed using **GitHub Pages**. Here’s the workflow:

1.  **Setup**: The project was initialized with Vite (`npm create vite@latest`), which provides a fast development environment and build tooling[reference:7].
2.  **Development**: The entire application was developed locally using React components, with assets stored in the `assets` folder[reference:8].
3.  **Build**: A production build is created by running `npm run build`. This process optimizes the code into static files (HTML, CSS, JS) in a `dist` folder, ready for deployment[reference:9].
4.  **Deployment (CI/CD)**: The project uses a **GitHub Actions** workflow for Continuous Integration and Continuous Deployment (CI/CD).
    *   On every `git push` to the `main` branch, the action automatically runs `npm install` and `npm run build`.
    *   It then deploys the contents of the new `dist` folder to the `gh-pages` branch.
5.  **Hosting**: **GitHub Pages** is configured to serve the website from the `gh-pages` branch, making it publicly accessible[reference:10].

This automated pipeline ensures the live site is always up-to-date with the latest code in the repository.
