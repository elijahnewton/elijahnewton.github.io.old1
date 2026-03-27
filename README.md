# Weekend IT Tutorials Hub

A mobile-first, static web application for programming and IT education. Students can follow structured learning paths, access interactive resources, and track their progress — all from a browser with no back-end required.

---

## 📋 Overview

The Weekend IT Tutorials Hub provides self-paced learning content for topics such as C Programming and Web Development. Content is stored as JSON and Markdown files that are loaded dynamically by the front-end, making the platform easy to extend and deploy anywhere static files can be served.

---

## 🚀 Features

- **Structured Learning Path** — Step-by-step guided tutorials organised into lessons
- **Interactive Resources** — Videos, code templates, and downloadable assets
- **Progress Tracking** — Saves and displays course-completion progress locally in the browser
- **Mobile-First Design** — Responsive layout optimised for phones, tablets, and desktops
- **Achievement System** — Gamified learning experience with badges and streaks
- **Accessible UI** — Keyboard navigation, screen-reader support, and high-contrast mode

---

## 📁 Project Structure

```
.
├── index.html                   # Main entry point
├── structured-learning.html     # Structured learning path page
├── interactive-resources.html   # Interactive resources page
├── progress.html                # Progress tracking page
├── components/
│   └── header.html              # Shared page header component
├── styles/
│   ├── main.css                 # Global styles
│   ├── components.css           # Component-specific styles
│   └── responsive.css           # Responsive / breakpoint styles
├── scripts/
│   ├── main.js                  # Application bootstrap
│   ├── navigation.js            # Client-side routing and navigation
│   ├── content-loader.js        # Loads content from JSON/Markdown files
│   ├── progress-tracker.js      # User progress persistence (localStorage)
│   └── mobile-handler.js        # Mobile gesture and touch handling
├── content/
│   ├── topics/
│   │   ├── learning-paths.json  # Defines available learning paths
│   │   ├── c-programming/
│   │   │   ├── meta.json        # Course metadata
│   │   │   ├── lesson-1.md … lesson-12.md
│   │   │   └── exercises.json   # Practice exercises
│   │   └── web-development/
│   │       ├── meta.json
│   │       └── lesson-1.md … lesson-6.md
│   └── resources/
│       ├── resources.json
│       └── interactive-resources.json
└── weekend-it-tutorials/        # Mirror / distribution copy of the above
```

---

## 🛠️ Getting Started — Run Locally

Because the app fetches local files at runtime, it must be served over HTTP (opening `index.html` directly in a browser will not work).

1. **Clone or download** this repository.
2. **Start a local web server** from the project root:

   ```bash
   # Python 3
   python -m http.server 8000

   # Node.js
   npx http-server

   # PHP
   php -S localhost:8000
   ```

3. **Open your browser** and navigate to `http://localhost:8000`.

---

## 🎯 Usage

### For Students

1. Open the site in your browser.
2. Choose a learning mode — **Structured Learning** or **Interactive Resources**.
3. Select a course and complete lessons in order for the best experience.
4. Use the code examples and exercises to practise what you learn.
5. Check the **Progress** page to see your completion stats and achievements.

### For Educators

- All learning content is stored in plain JSON and Markdown files under `content/`.
- Add a new course by creating a folder in `content/topics/` with a `meta.json` and lesson files, then register it in `content/topics/learning-paths.json`.
- Add new interactive resources by editing `content/resources/resources.json` or `interactive-resources.json`.
- Update styles in `styles/` and shared UI in `components/`.

---

## 🤝 Contributing

Contributions are welcome!

1. Fork this repository.
2. Create a feature branch (`git checkout -b feature/my-improvement`).
3. Make your changes and test them on multiple screen sizes.
4. Open a pull request describing what you changed and why.

Please follow the existing content and code structure so that the project stays consistent.

---

## 📄 License

No license specified.

---

## 🆘 Support / Contact

If you run into issues:

- Make sure you are serving the files via an HTTP server (see [Getting Started](#️-getting-started--run-locally)).
- Open your browser's developer console for error messages.
- Verify that all JSON files are valid (use a tool such as [JSONLint](https://jsonlint.com)).

For questions or feedback, contact the project maintainer:
**Email:** musiitwaelijah@gmail.com
