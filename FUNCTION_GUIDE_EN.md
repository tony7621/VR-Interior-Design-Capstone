# 📖 VR Interior Design System - Functional Guide & UI Walkthrough

This document details the core functionalities and user interfaces of the system, showcasing the integration of 2D spatial algorithms, VR immersion, and AI-driven recommendations.

---

### 1. Spatial Geometry Algorithm & Auto-Floor Generation
* **Core Logic**: The system tracks 2D wall rendering in real-time. Upon detecting a fully enclosed polygon, the algorithm calculates the boundaries and automatically generates the corresponding floor mesh.
* **Complex Layout Support**: Capable of identifying multiple independent enclosed regions simultaneously, perfectly adapting to complex interior layouts such as L-shaped or multi-room configurations.

![Auto-Floor Generation](assets/multi_room_floor.png)

---

### 2. Multi-Perspective Switching & VR Immersion
* **Seamless View Switching**: Offers 2D top-down planning, 3D volumetric inspection, and First-Person Shooter (FPS) keyboard roaming modes to fulfill design review needs at various stages.
* **SteamVR Integration**: Supports VR headsets and spatial controllers. Users can walk, interact, and inspect furniture details at a true 1:1 physical scale.

![VR and Multi-Perspective](assets/vr_gameplay.png)

---

### 3. AI Generation & Semantic Recommendation Engine
* **Natural Language Spatial Generation**: Integrated with the OpenAI API. Users input simple natural language prompts (e.g., *"Japanese-style bedroom"*), and the system parses the semantics to automatically generate a preliminary spatial layout.

![AI Prompt Interface](assets/ai_prompt.png)

* **Smart Asset Recommendation**: Based on the user's design style keywords, the system retrieves and recommends the best-matching furniture, wallpapers, and floor textures from a comprehensive database, significantly reducing asset-searching time.

![AI Recommendation](assets/ai_recommendation.png)

---

### 4. Data Persistence & Real-Time Cost Management
* **JSON Serialization**: Completely serializes and saves wall coordinates, material settings, and furniture transforms.
* **Multi-Version Management**: Features an independent "Previous Designs" dashboard. It automatically generates thumbnail previews, timestamps, and calculates the total furniture count and **real-time estimated budget (Total Price)** for each saved design, enabling synchronized design and cost control.

![Data Persistence and Costing](assets/version_management.png)
