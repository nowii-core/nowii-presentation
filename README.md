# nowii — Built from zero
A 60-second interactive WebGL film and high-performance visual experience built for simplicity.
A clean web presentation powered by vanilla WebGL, HTML5 Canvas 2D, and JavaScript, with custom particle typography and procedural audio narration.

[Overview](#overview) | [Features](#features) | [Quick Start](#quick-start) | [Structure](#structure) | [Development](#development) | [License](#license)

---

## Overview
**nowii — Built from zero** is a lightweight web presentation designed around simplicity, responsiveness, and pure performance.  
Built with standard web technologies, it keeps the project structure straightforward and easy to understand. Its modular architecture separates the visual presentation, fluid WebGL background shaders, custom particle physics, and browser speech narration into a single, dependency-free codebase.  
With no build system required for basic development, nowii provides a simple starting point for building and experimenting with modern, zero-dependency web experiences.

---

## Features
- **Zero-Dependency Architecture** — Built entirely with standard web technologies without requiring external frameworks or libraries.
- **WebGL Fluid Background** — Features a custom WebGL fragment shader rendering dynamic procedural fluid colors.
- **Particle Typography** — Text is converted into interactive pixel-particle physics with multiple entrance and shatter transition effects.
- **Procedural Narration & Fallback** — Integrates audio narration clips with automatic fallback to the Web Browser SpeechSynthesis API.
- **Built-in Screen Recorder** — Allows users to record and download the 60-second visual presentation in WebM format directly from the browser.
- **Responsive Canvas Layout** — Automatically scales particle graphics, font sizes, and layout parameters based on screen resolution and DPR.
- **Cross-Platform** — Runs in modern browsers across supported desktop and mobile operating systems.
- **Developer-Friendly** — A straightforward single-file structure that makes extending the visual components easier.

---

## Preview

**Live Demo:** [https://nowii-core.github.io/nowii-presentation/](https://nowii-core.github.io/nowii-presentation/)

---

## Tech Stack

| Technology | Purpose |
| :--- | :--- |
| **HTML5** | Application structure and Canvas containers |
| **CSS3** | Modern typography, subtle glassmorphism, and keyframe animations |
| **JavaScript (ES6+)** | Animation loop, particle physics, and audio timeline logic |
| **WebGL 2D** | Procedural fluid shader background and color transitions |
| **HTML5 Canvas 2D** | High-performance particle typography and visual graphics |
| **Web Audio / SpeechSynthesis** | Synchronized audio playback and browser narration fallback |

* **Dependencies:** None required for the basic application.

---

## Quick Start

### Requirements
- A modern web browser supporting WebGL and HTML5 Canvas.
- **Visual Studio Code** or another code editor.
- **Live Server** or another local development server for testing local audio files.

### Run Locally
1. **Clone the repository**
   ```bash
   git clone https://github.com/nowii-core/nowii-presentation.git
   ```
2. **Enter the project directory**
   ```bash
   cd nowii-presentation
   ```
3. **Open the project**
   ```bash
   code .
   ```
4. **Start the application**  
   Open `index.html` using the **Live Server** extension in Visual Studio Code.  
   Alternatively, open the `index.html` file directly in your browser to preview the basic visual experience.

> **Note:** Audio narration loading (`audio/*.wav`) requires a trusted local server environment (such as `localhost` or Live Server) due to browser CORS policies.

---

## Project Structure

```text
nowii-presentation/
├── index.html       # Main application entry point (HTML, WebGL, Canvas & JS logic)
├── logo.png         # Fallback logo graphic used inside particle scenes
├── README.md        # Project documentation
└── audio/           # Narration audio clips folder (0.wav to 9.wav)
```

---

## Customization

nowii's straightforward structure makes it easy to adapt the visual experience to your needs.

- **Interface & Text:** Edit the `S` array inside `index.html` to update scene headlines, timeline triggers, sub-captions, and voice scripts.
- **Design & Colors:** Modify the `tint` array in the script to change the WebGL background fluid color palettes per scene.
- **Particle Dynamics:** Adjust particle strides, explosion velocities, and transition timing inside `buildPhrase()` and `drawPhrase()`.
- **Branding:** Replace `logo.png` to update the mark used during scenes with bounce animation effects.

---

## Development

nowii is designed to be easy to work with using a minimal development setup.

### Recommended Workflow
1. Open the project in your preferred editor.
2. Start a local development server (e.g., Live Server).
3. Modify the HTML, CSS, WebGL shader code, or timeline data.
4. Refresh the browser to test your changes.
5. Verify canvas responsiveness, text particle rendering, and audio timing.

---

## Security & Privacy

nowii uses standard browser technologies and does not require a framework or package installation for its basic operation.  
Security and privacy depend on the application's actual implementation. Review any external audio requests, canvas recording permissions, and browser compatibility before deploying the application publicly.

---

## License

No license has been specified in the provided project description.  
If you intend to distribute nowii as an open-source project, add a `LICENSE` file and update this section accordingly.

---

## Contact & Support

- **Maintainer:** [@nowii-core](https://github.com/nowii-core)
- **Repository:** [https://github.com/nowii-core/nowii-presentation](https://github.com/nowii-core/nowii-presentation)
- **Issues & Feature Requests:** Open an issue in the repository once configured.

*Developed by nowii-core.*
