# INSTITUTO TECNOLÓGICO DE PACHUCA
## Ingeniería en Sistemas Computacionales
## Graficación
### 3.7 Desarrollo de escenarios VR
### Autores: 
### Aguilar Pérez Nahum
### Contla Martínez Kevin Bertín
### Ronaldo Olvera Jiménez 
### Santiago Padilla Rubén
### Fecha de entrega: 1 de diciembre de 2025
# graf-threejsEscenario3D-VR

🫧 **OXYVERSE VR**  
Oxyverse VR Banner Three.js WebXR

## Virtual Experience of an Oxygenation Factory

An interactive Virtual Reality application developed with Three.js, WebXR, and Cannon.js.

🎮 Live Demo • 📖 Documentation • 🐛 Report Bug

----------

## 📋 Table of Contents

-   Description
    
-   Features
    
-   Technologies
    
-   Installation
    
-   VR Controls
    
-   Project Structure
    
-   Developers
    
-   License
    

----------

## 🎯 Description

Oxyverse VR is an immersive virtual reality experience that simulates the interior of an industrial oxygenation plant. Users can explore different equipment and machinery, interact with objects through raycasting, and learn about the industrial oxygen production process through informative audio clips.

This project was developed as part of Activity 3.7: VR Scenario Development, using modern web technologies to create a fully functional educational and interactive experience on WebXR-compatible browsers.

----------

## ✨ Features

🥽 **Full VR Experience:** Compatible with Meta Quest 2/3, HTC Vive, and other WebXR devices  
🎮 **Intuitive Controls:** Movement with left joystick, rotation with right joystick  
🔦 **Raycast System:** Point at objects to get real-time information  
🎵 **Interactive Audio:** Every machine plays informational audio when pointed at  
⚙️ **Realistic Physics:** Collision system powered by Cannon.js  
🏭 **Detailed 3D Models:**

-   Complete oxygenation plant
    
-   Forklift
    
-   Industrial robot
    
-   Electric generator (Power Plant)
    
-   Warehouse shelving unit
    
-   Multiple industrial machines (Cold Box, Air Compressor, etc.)
    

🌅 **HDR Lighting:** Realistic environment with HDRI maps

----------

## 🛠️ Technologies

Technology

Version

Use

Three.js

0.164.1

3D graphics engine

WebXR

Latest

Virtual Reality API

Cannon.js

0.20.0

Physics engine

GLTF/GLB

2.0

3D model format

Draco Loader

Latest

Geometry compression

OrbitControls

Three.js

Desktop navigation

----------

## 🚀 Installation

### Prerequisites

-   WebXR-compatible browser (Chrome, Edge, Firefox Reality)
    
-   VR headset (Meta Quest, HTC Vive, etc.)
    
-   Local web server (for development)
    

### Installation Steps

**Clone the repository**

`git clone https://github.com/tu-usuario/oxyverse-vr.git cd oxyverse-vr` 

**Install a local server (choose one):**

`# Option  1: Python
python -m http.server  5500 # Option  2: Node.js (http-server)
npx http-server -p 5500 # Option  3: VS Code Live Server # Install "Live Server" extension  and right-click > "Open with Live Server"` 

**Open in the browser**

`http://localhost:5500/inicio.html` 

Connect your VR headset and click **"Start VR Experience"**.

----------

## 🎮 VR Controls

### Movement Controls

Control

Action

Left Joystick

Move forward/backward/left/right

Right Joystick (Horizontal)

Rotate 45° left/right

Right Trigger

Enable/Disable Raycast

Point with Raycast

Display equipment information (audio playback)

### Desktop Controls (Development Mode)

-   Mouse: Look around
    
-   Scroll: Zoom
    
-   Click + Drag: Orbit camera
    

----------

## 📁 Project Structure

`GRAF-THREEJSESCENARIO3D+VR/
│
├── index.html # Main VR application with loader ├── indexInicio.html # Welcome page ├── main.js # Core VR application logic │
└── assets/ # Project assets │
├── Forklift.glb # 3D Model: Forklift ├── industrial_robot.glb # 3D Model: Industrial robot ├── industrial_sunset_puresky_1k.hdr # HDRI lighting map ├── Oxygenation.glb # 3D Model: Oxygenation plant (visual) ├── Oxygenation_Collidors.glb # 3D Model: Plant colliders ├── Power_Plant.glb # 3D Model: Electric generator ├── Warehouse_Shelving_Unit.glb # 3D Model: Warehouse shelving unit │
├── Audio/ # Audio files │   ├── After_Cooler.mp3
│   ├── Air_Compressor.mp3
│   ├── Air_Expander.mp3
│   ├── Air_Filter.mp3
│   ├── Carbon_Dioxide_Drying_Unit.mp3
│   ├── Cold_Box.mp3
│   ├── Cylinder_Filling_Ramp.mp3
│   ├── Forklift.mp3
│   ├── Freon_Cooler.mp3
│   ├── Industrial_Robot.mp3
│   ├── Liquid_Oxygen_Pump.mp3
│   ├── Moisture_Absorber.mp3
│   ├── Nitrogen_Cooler.mp3
│   ├── Oil_Absorber.mp3
│   ├── Power_Plant.mp3
│   ├── Purger.mp3
│   ├── Regeneration_Heater.mp3
│   └── Warehouse_Shelving_Unit.mp3
│
└── Images/ # Graphic resources └── Icon.png # App icon` 

----------

## 👥 Developers

This project was developed by students from the National Technological Institute of Mexico as part of the Virtual Reality course:

Name

Student ID

GitHub

Aguilar Pérez Nahum

23200135

@usuario1

Contla Martínez Kevin Bertín

23200139

@usuario2

Olvera Jiménez Ronaldo

23200151

@usuario3

Santiago Padilla Rubén

23200158

@usuario4

----------

## 📝 Academic Activity

📚 **Activity 3.7:** VR Scenario Development  
🏫 **Institution:** National Technological Institute of Mexico  
📅 **Year:** 2025  
👨‍🏫 **Course:** Virtual Reality

----------

## 🔧 Technical Features

### Collision System

-   Cannon.js physics engine for collision detection
    
-   Custom colliders for each object
    
-   Player collision capsule with 0.95 damping
    

### Optimizations

-   Asynchronous model loading with LoadingManager
    
-   Draco compression for geometries
    
-   Optimized manual colliders
    
-   Toggleable debug mode for development
    

### Spatial Audio

-   3D audio system with THREE.Audio
    
-   Automatic playback when pointing at objects
    
-   Volume and loop control
    

----------

## 🐛 Known Issues

-   On some mobile browsers, audio may not autoplay
    
-   Initial loading may be slow on weak networks
    
-   Requires HTTPS for production (WebXR requirement)
    

----------

## 🚀 Roadmap

-   Add more industrial machinery
    
-   Inventory system
    
-   Multiplayer mode
    
-   Translations (ES/EN)
    
-   Optimization for Quest 2 standalone
    
-   Interactive tutorial
    

----------

## 📄 License

This project is for academic use. All rights reserved © 2025

----------

## 🙏 Acknowledgments

-   Three.js Team – For the amazing graphics engine
    
-   Khronos Group – For the WebXR standard
    
-   Sketchfab Community – For the base 3D models
    

⭐ If you enjoyed this project, leave a star!
