# 360 Tour

A lightweight, web-based 360° virtual tour built with plain JavaScript, CSS, and HTML. This project provides an easy starting point to create immersive panoramic tours with scenes, hotspots, and basic navigation — no heavy frameworks required.

Languages
- JavaScript: 58.1%
- CSS: 33.4%
- HTML: 8.5%

---

## Table of Contents
- [Demo](#demo)
- [Features](#features)
- [Tech Stack](#tech-stack)
- [Getting Started](#getting-started)
  - [Prerequisites](#prerequisites)
  - [Install & Run](#install--run)
- [Usage](#usage)
- [Project Structure](#project-structure)
- [Adding/Editing Scenes & Assets](#addingediting-scenes--assets)
- [Development Tips](#development-tips)
- [Contributing](#contributing)
- [License](#license)
- [Credits](#credits)
- [Contact](#contact)

---

## Demo
If a live demo is available, add the link here:

Live Demo: TODO — replace this with your deployed URL (e.g., GitHub Pages)

---

## Features
- Display 360° panoramic scenes in the browser
- Scene navigation and basic controls (pan/zoom)
- Hotspots to jump between scenes or show information
- Simple, framework-free codebase for easy customization
- Small footprint: HTML/CSS/JavaScript only

---

## Tech Stack
- JavaScript (core logic and interactions)
- CSS (styling and layout)
- HTML (markup and structure)

---

## Getting Started

### Prerequisites
- A modern web browser (Chrome, Firefox, Edge, Safari)
- Optional: Node.js & npm if you plan to use local dev tooling

### Install & Run

1. Clone the repository
```bash
git clone https://github.com/nramchandra504-ai/360-tour.git
cd 360-tour
```

2. If the project has a `package.json` and dependencies:
```bash
npm install
npm start
```
(Replace `npm start` with the actual start script if different.)

3. If there are no build scripts, you can serve the project with a simple static server:

- Using Python (works in repo root):
```bash
# Python 3
python -m http.server 8000
# then open http://localhost:8000 in your browser
```

- Using npx serve:
```bash
npx serve .
# then open the printed local URL
```

- Or open `index.html` directly in the browser (some features like fetching assets may require a server).

---

## Usage
- Open the project in your browser or run a local server as shown above.
- Use the UI controls (if provided) to move between scenes and interact with hotspots.
- Replace demo panoramas in the assets folder with your own images to create custom tours.

---

## Project Structure (Suggested)
The exact structure may vary — adjust to your repo contents.

```
360-tour/
├─ assets/
│  ├─ panoramas/        # 360° images (equirectangular)
│  └─ thumbnails/
├─ css/
│  └─ styles.css
├─ js/
│  └─ app.js            # main tour logic
├─ index.html
└─ README.md
```

---

## Adding/Editing Scenes & Assets
- Put high-resolution equirectangular images (JPEG/PNG) into `assets/panoramas`.
- Scenes might be defined in a JSON file or directly in `app.js` depending on implementation. A simple scene object might look like:

```js
{
  id: "lobby",
  title: "Main Lobby",
  panorama: "assets/panoramas/lobby.jpg",
  hotspots: [
    { x: 0.2, y: 0.4, type: "link", target: "gallery", label: "Go to Gallery" },
    { x: 0.6, y: 0.5, type: "info", text: "This is the main reception." }
  ]
}
```

- Update the scene list in the code and restart the server (if needed) to see changes.

---

## Development Tips
- Use browser devtools to inspect errors and asset paths.
- For editing and quick reloads, use the Live Server extension in VS Code.
- Optimize panorama images (compress and use appropriate resolutions) to reduce load time.
- If adding large images, consider lazy-loading panoramas or using progressive loading.

---

## Contributing
Contributions are welcome! A suggested workflow:
1. Fork the repository
2. Create a feature branch: `git checkout -b feat/my-feature`
3. Commit your changes: `git commit -m "Add my feature"`
4. Push to your fork: `git push origin feat/my-feature`
5. Open a pull request describing your changes

Please open issues for bugs or feature requests and include steps to reproduce.

---

## License
This repository does not include a license by default. To apply a license (e.g., MIT), create a `LICENSE` file. Example MIT header:

```
MIT License

Copyright (c) 2025 Your Name

Permission is hereby granted...
```

Replace with your preferred license or let me know which license you'd like and I can add one.

---

## Credits
- Built with vanilla JavaScript, CSS, and HTML.
- Thanks to open-source libraries or resources used (list them here if any).

---

## Contact
Maintainer : osmania


If you'd like, I can:
- generate example scene JSON and sample panoramas (placeholders),
- add a ready-to-use start script (package.json),
- create a GitHub Pages deploy workflow.

Tell me which of the above you'd like next and I will create the files.
