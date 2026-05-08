# Solar System Simulation - Three.js Project

## Overview

This project is a 3D interactive simulation of the Solar System built using **Three.js**.  
It was developed as part of a Computer Graphics seminar assignment and demonstrates key concepts of 3D rendering in the browser using WebGL.

The scene includes the Sun, seven planets with textures, an asteroid with custom geometry, and a particle system simulating stars in space.

---

## Features

### 🌞 Solar System
- The Sun is placed at the center of the scene.
- Seven planets orbit around the Sun:
  - Mercury
  - Venus
  - Earth
  - Mars
  - Jupiter
  - Saturn
  - Neptune

Each planet has:
- Realistic texture mapping
- Individual orbital speed
- Scaled radius based on relative size

---

### 🌍 Planet Orbits
- Orbital motion is simulated using **pivot objects (Object3D)**.
- Each planet rotates around its own pivot to create circular orbit behavior.

---

### ✨ Starfield (Particles System)
- Background stars are implemented using **BufferGeometry** and **PointsMaterial**.
- 2000 randomly positioned particles simulate a space environment.

---

### ☄️ Custom Asteroid
- The asteroid is created using **custom geometry (procedural generation)**.
- Vertices are randomly generated to form an irregular shape.
- Demonstrates manual mesh construction in Three.js.

---

### 🎮 User Interaction

The application supports real-time interaction:

#### Mouse Controls
- Implemented using **OrbitControls**
- Allows zoom, rotation, and scene navigation

#### Keyboard Controls
- ↑ Increase orbital speed
- ↓ Decrease orbital speed
- Space → Pause/Resume animation

#### GUI Controls (dat.GUI)
- Adjust orbital speed
- Toggle animation pause
- Change background color

---

### 💡 Lighting
- A **PointLight** simulates the Sun as a light source.
- **Ambient light** ensures basic visibility of objects.

---

### 🎥 Animation System
- Built using `requestAnimationFrame`
- Smooth real-time updates of:
  - Planet orbits
  - Asteroid rotation
  - Starfield movement

---

## Project Structure
/project-folder
│
├── index.html
├── lib/
│ ├── three.js
│ ├── OrbitControls.js
│ └── dat.gui.js
│
├── textures/
│ ├── mercury.jpg
│ ├── venus.jpg
│ ├── earth.jpg
│ ├── mars.jpg
│ ├── jupiter.jpg
│ ├── saturn.jpg
│ └── neptune.jpg
│
└── README.md

---

## Technologies Used

- Three.js (WebGL 3D engine)
- JavaScript (ES6)
- HTML5 / CSS3
- dat.GUI (UI controls)

---

## How to Run the Project

1. Open the project folder in VS Code or another editor.
2. Run the project using a local server (e.g. Live Server).
3. Open `index.html` in the browser.

> Important: Textures will not load correctly if opened directly via `file://`. Always use a local server.

---

## Learning Outcomes

This project demonstrates:
- 3D scene creation in Three.js
- Use of geometries and materials
- Texture mapping
- Particle systems
- Camera controls
- Animation loop design
- User interaction via mouse and keyboard
- Procedural geometry creation

---

## Author
Student Project - Computer Graphics Course 