# Nextbot: The Office 🏃‍♂️💨

A self-contained, browser-based survival horror game built entirely in a single HTML file. You are trapped in an abandoned, fluorescent-lit office complex. A corrupted Nextbot entity is hunting you down. 

It knows where you are. It does not stop. **Run.**

## ✨ Features
* **100% Self-Contained:** No external images, assets, or models required. The Nextbot's terrifying face is programmatically generated using the HTML5 Canvas API so it will never break due to dead links or CORS errors.
* **Three.js Graphics:** Dynamic point lights, flickering fluorescent bulbs, fog, and shiny linoleum office floors.
* **Stamina System:** You can sprint, but your stamina will drain quickly. Manage it carefully.
* **Procedural Audio:** Utilizes the Web Audio API to create a dynamic, heart-pounding chase sound that gets faster and louder as the Nextbot gets closer.

## 🎮 Controls

* **W, A, S, D:** Move
* **Mouse:** Look around
* **Shift (Hold):** Sprint
* **Click:** Lock mouse and start the game

*Watch your stamina bar at the bottom left. If it turns red, you are out of breath and will be forced to walk until it regenerates.*

## 🚀 How to Run Locally

Because this game uses JavaScript ES Modules (`type="module"`) to load the Three.js library from a CDN, **you cannot just double-click the HTML file**. Browsers will block the scripts due to local CORS security policies.

You need to run a quick local web server. Here are the easiest ways:

### Option 1: VS Code (Recommended)
1. Install the [Live Server](https://marketplace.visualstudio.com/items?itemName=ritwickdey.LiveServer) extension in Visual Studio Code.
2. Open `index.html`.
3. Click the **"Go Live"** button in the bottom right corner of VS Code.

### Option 2: Python
Open your terminal/command prompt, navigate to the folder containing `index.html`, and run:
```bash
python -m http.server
