# IIC-AIR 2027 - 1st Indraprastha International Conference

Official flagship website for the **1st Indraprastha International Conference on Artificial Intelligence, IoT and Robotics (IIC-AIR 2027)**.

The conference brings together global researchers, students, faculty, and industry professionals to present cutting-edge developments in core technological domains.

---

## 📅 Conference Details

- **Workshops & Tutorials**: November 5, 2026
- **Main Conference**: November 6–7, 2026
- **Venue**: Guru Gobind Singh Indraprastha University (GGSIPU), East Delhi Campus, Surajmal Vihar, Delhi - 110032, India

---

## 🛠️ Technology Stack

This project is built using modern, high-performance web standards:
- **Framework**: [Next.js 16 (App Router)](https://nextjs.org/)
- **Runtime & UI**: [React 19](https://react.dev/)
- **Styling**: [Tailwind CSS v4](https://tailwindcss.com/)
- **Animations**: [Framer Motion](https://www.framer.com/motion/)
- **Scrolling**: [Lenis Smooth Scroll](https://lenis.darkroom.engineering/)
- **Language**: [TypeScript](https://www.typescriptlang.org/)

---

## 🚀 Getting Started

### Prerequisites

Ensure you have Node.js 20+ installed on your system.

### Installation

1. Install all dependencies:
   ```bash
   npm install
   ```

2. Start the local development server:
   ```bash
   npm run dev
   ```

3. Open [http://localhost:3000](http://localhost:3000) in your browser.

### Production Build

To compile and export the application as a production-ready static site:
```bash
npm run build
```
This command generates an optimized static export in the `./out` directory.

---

## ⚙️ CI/CD & Deployment

This repository is equipped with a GitHub Actions workflow for automatic deployment:

- **Trigger**: Every push to the `main` branch.
- **Workflow**: Runs lint checks (`npm run lint`), compiles the static build (`npm run build`), copies custom Apache server-side rewrite rules (`.htaccess` for clean routes and HTTPS redirection), and deploys the build output to cPanel hosting via FTP.
- **Setup Details**: For instructions on configuring cPanel and GitHub repository secrets, please refer to the [Deployment Guide](file:///Users/sheelendra/Documents/zed/acm-conf/DEPLOYMENT.md).

---

## ♿ Accessibility & Design Principles

- **Academic First**: Visual clarity and authoritative presentation of tracks, speakers, and milestones.
- **Accessibily-Compliant**: Built to WCAG level AA guidelines, supporting high-contrast displays, screen readers, and `prefers-reduced-motion` safety.
- **Responsive Layout**: Fluid design tailored for mobile, tablet, and desktop screens.
