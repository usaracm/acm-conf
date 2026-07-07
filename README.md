# IIC-AIR 2027 - 1st Indraprastha International Conference

Official flagship website for the **1st Indraprastha International Conference on Artificial Intelligence, IoT and Robotics (IIC-AIR 2027)**.

The conference brings together global researchers, students, faculty, and industry professionals to present cutting-edge developments in core technological domains.

---

## Conference Details

* **Workshops & Tutorials**: January 13, 2027
* **Main Conference**: January 14-15, 2027
* **Venue**: Guru Gobind Singh Indraprastha University (GGSIPU), East Delhi Campus, Surajmal Vihar, Delhi - 110032, India

---

## Technology Stack

This project is built using modern, high-performance web standards:
* **Framework**: Next.js 16 (App Router)
* **Runtime & UI**: React 19
* **Styling**: Tailwind CSS v4
* **Animations**: Framer Motion
* **Scrolling**: Lenis Smooth Scroll
* **Language**: TypeScript
* **Data Verification**: Zod

---

## File Structure

Below is the directory layout showing the clean file architecture and core modular parts:

```text
.
├── .github/              # GitHub Action workflows
│   └── workflows/
│       └── deploy.yml    # Automated CI/CD deployment pipeline
├── app/                  # Next.js App Router page layouts and routing
│   ├── (marketing)/      # Core conference views (Home, Committee, Dates, Registration, Tracks, Venue)
│   ├── favicon.ico       # Website browser icon
│   ├── globals.css       # Tailored styling rules and design tokens
│   └── layout.tsx        # Base page layout structure
├── components/           # Modular visual components
│   ├── home/             # Hero, Stats Grid, and landing components
│   ├── layout/           # Shared Navigation bar and Footer
│   ├── shared/           # Countdown clock and Timelines
│   └── tracks/           # Interactive track grids and cards
├── content/              # JSON-based content (Single Source of Truth)
│   ├── committee.json    # Committee listing and structural roles
│   ├── dates.json        # Deadlines and schedules
│   ├── news.json         # Announcements feed
│   ├── speakers.json     # Keynote speaker directory
│   └── tracks.json       # Technical tracks and scopes
├── lib/                  # Application helper utilities and validation schemas
│   ├── content.ts        # Content loading abstraction layer (Zod validation)
│   └── utils.ts          # Styling join helpers
├── public/               # Public assets and configurations
│   ├── .htaccess         # cPanel Apache web server rules (HTTPS and clean routing)
│   ├── GGSIPU_LANDSCAPE.png
│   └── BLUE WITH WHITE TEXT.png
└── DEPLOYMENT.md         # Step-by-step cPanel and GitHub Secrets guide
```

---

## Getting Started

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

## CI/CD & Deployment

This repository is equipped with an automated deployment pipeline:

* **Trigger**: Every push to the `main` branch.
* **Process**: Runs lint checks (`npm run lint`), compiles the static build (`npm run build`), copies custom Apache server-side rewrite rules (`.htaccess` for clean routing and HTTPS redirection), and deploys the build output to cPanel hosting via FTP.
* **Deployment Instructions**: For details on setting up credentials, directory overrides, and server-side configurations, see the [Deployment Guide](file:///Users/sheelendra/Documents/zed/acm-conf/DEPLOYMENT.md).

---

## Accessibility & Design Principles

* **Academic First**: Focuses on structured information, high readability, and clean visual typography.
* **Accessibility Compliant**: Adheres to WCAG Level AA requirements with proper text-to-background contrast ratios and support for keyboard-only navigation.
* **Motion with Purpose**: Implements smooth transitions using Framer Motion and Lenis scroll, respecting user preferences via `prefers-reduced-motion` hooks.
