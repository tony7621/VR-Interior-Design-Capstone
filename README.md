# 🏆 VR Interior Design System & AI Spatial Assistant (Capstone Project)

> **Award**: First Place Outstanding Award
> **Institution**: National Dong Hwa University – Dept. of Information Management
> **Role**: Team Lead (5-Member Cross-Functional Development Team)

![Unity](https://img.shields.io/badge/Unity-2021_LTS-black?logo=unity)
![SteamVR](https://img.shields.io/badge/SteamVR-OpenXR-blue)
![AI](https://img.shields.io/badge/OpenAI-API_Integration-412991?logo=openai)
![Architecture](https://img.shields.io/badge/Architecture-Modular_OOP-orange)

## 📌 1. Project Overview
This project is an advanced, integrated interior design and spatial planning platform built to bridge the gap between abstract 2D floor plans and 3D immersive environments[cite: 29]. By combining **real-time spatial topology calculations, multi-perspective switching, SteamVR spatial immersion, and OpenAI-driven generative features**, the system allows both novices and professionals to seamlessly design, visualize, and budget room layouts within a single application[cite: 29].

---

## ⚙️ 2. Core Functional Modules

### ① Architectural & Spatial Engine (Walls & Floors)
* **Wall Creation & Dynamic Editing**: Users can construct walls by specifying start and end points in a 2D grid. The system processes topological connections in real-time, instantly recalculating spatial structures upon any wall addition, movement, or deletion to prevent geometric misalignment[cite: 29].
* **Smart Closed-Loop Detection & Auto-Floor Generation**: Implements a geometric validation algorithm that continuously checks wall connectivity. Floor meshes are automatically instantiated *only* when a closed loop is detected, eliminating manual modeling errors and fully supporting complex L-shaped or multi-room configurations[cite: 29].

### ② Multi-Perspective & VR Immersion
* **2D Layout View**: Provides a top-down planar grid perspective tailored for rapid structural layout and wall planning[cite: 29].
* **3D Spatial View**: Enables orthogonal and perspective-based volumetric inspection to evaluate height proportions and furniture placement[cite: 29].
* **First-Person (FPS) Roaming Mode**: Simulates natural indoor navigation using WASD keyboard controls to experience human-scale spatial flow[cite: 29].
* **VR Immersive Mode**: Integrated with **SteamVR and Unity XR**, allowing users to wear VR headsets and interact with virtual furniture at a true 1:1 physical scale using spatial controllers[cite: 29].

### ③ AI-Driven Design & Recommendation Engine
* **AI Spatial Generation**: Parses natural language user prompts (e.g., *"Japanese-style bedroom"*) via the OpenAI API to procedurally generate preliminary room layouts and furniture configurations[cite: 29].
* **AI Furniture Recommendation**: Automatically queries and filters relevant furniture from a comprehensive catalog based on semantic intent and keyword matching[cite: 29].
* **AI Wallpaper & Material Recommendation**: Recommends contextually matched wall textures and flooring styles to accelerate the design decision-making pipeline[cite: 29].

### ④ Interactive Furniture & Material Customization
* **Advanced Catalog & Search**: Built-in searchable database supporting filtering by brand, category, and keywords across 16 pages of assets[cite: 29].
* **Constraint-Based Placement & Editing**: Drag-and-drop instantiation with automatic floor snapping to prevent floating objects. Supports axis rotation, height elevation adjustments for wall-mounted items, and quick deletion via the `Delete` key[cite: 29].
* **Material Management**: Granular texture replacement for individual or all walls/floors, backed by single-step and global undo/reset mechanisms[cite: 29].

### ⑤ Data Persistence & Real-Time Cost Estimation
* **JSON-Based Serialization**: Persists wall topologies, material IDs, furniture transforms, and metadata into local structured JSON files[cite: 29].
* **Versioning & Thumbnail Management**: A dedicated management dashboard featuring thumbnail previews, timestamps, item counts, and real-time total price calculations (`總價`) to support multi-version design comparisons[cite: 29].

---

## 👥 3. Team Leadership & My Contributions
As the **Team Lead of a 5-member cross-functional group**, my core responsibilities included:
* **System Architecture Design**: Established the modular OOP structure in Unity, defining the data flow between the spatial geometry engine, UI controllers, and local storage.
* **AI & NLP Integration**: Engineered the OpenAI API pipeline to handle natural language parsing for automated room layout generation and smart asset recommendations.
* **Git Version Control & Project Management**: Managed multi-branch collaboration, resolved complex scene merge conflicts (`.unity` binaries and prefabs), and delivered the project on schedule, earning the **First Place Outstanding Award (特優獎)**.

---

## 🛠️ 4. Tech Stack & Environment
* **Engine & Language**: Unity (2021 LTS), C#
* **VR Framework**: SteamVR, Unity XR Plugin
* **AI Integration**: OpenAI API
* **Data Layer**: Local JSON Serialization
* **Execution Environment**: Windows 10/11 (64-bit), recommended with dedicated GPU and SteamVR-compatible headset (e.g., HTC Vive series)

---
*Note: Due to commercial 3D asset licensing and academic IP policies, the complete Unity source code is private. Architectural specifications and documentation are available upon request.*
