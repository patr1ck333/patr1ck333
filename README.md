# Welcome to my Group Project Github! 👋 

I'm currently a student at the University of Waterloo studying Mechatronics (Class of 2026). I'm passionate about building scalable software, designing efficient systems, and bringing complex projects to life. 

## 🔒 Currently Building/Built (Private Repos)
### 1. 👗 DressCode: Digital Wardrobe Management (Android & Kotlin)
#### 📌 The Problem: "Closet Blindness"
DressCode was built to solve **closet blindness** i.e. the tendency for users to forget their physical inventory. This lack of visibility leads to redundant purchases, wasted time during daily styling, and underutilized wardrobe assets.

#### 🏗️ Architecture & Technical Stack

| Layer | Technology | Role |
| :--- | :--- | :--- |
| **Backend** | **Kotlin / Ktor** | High-concurrency server utilizing a **Layered Architecture** to ensure strict separation of concerns. |
| **Frontend** | **Android SDK / Jetpack Compose** | Modern, declarative UI built on the **MVVM (Model-View-ViewModel)** pattern for reactive state management. |
| **Database** | **PostgreSQL (Supabase)** | Managed relational database using **Row-Level Security (RLS)** to enforce data privacy at the schema level. |
| **Infrastructure** | **Supabase Auth & Storage** | Handles secure **OAuth** (Email/Google) and cloud-hosted asset management for wardrobe images. |
| **Testing** | **Testcontainers** | Utilized for robust integration testing by spinning up isolated PostgreSQL instances during the build process. |

<hr>

#### 🚀 Key Technical Achievements

##### 🤖 On-Device AI & Computer Vision
* **Background Removal**: Implemented pixel-by-pixel foreground segmentation using **Google ML Kit’s Subject Segmentation API**.
* **Privacy-First Processing**: All image processing occurs **on-device**, ensuring user data remains private while providing low-latency background removal for newly uploaded items.

##### 🗓️ Collaborative Planning & Social Logic
* **Invite-Code System**: Engineered a unique alphanumeric invite-code mechanism that allows users to join shared events and coordinate outfits in real-time.
* **Weather-Driven Logic**: Integrated a 3-day **Weather API** (with a season-neutral fallback) to surface relevant styling recommendations based on local forecasts.

##### ⚡ Optimized Performance & Scalability
* **Minimal Footprint**: Kept the local app storage footprint **under 500MB** by offloading high-resolution assets to cloud storage and leveraging in-memory caches.
* **Data Efficiency**: Architected the backend to use efficient **primary-key UUID lookups** and indexed server-side SQL filtering to ensure rapid page renders.
---
#### 📊 Strategic Trade-offs
* **Future-Oriented Priority**: We intentionally deprioritized historical outfit tracking to focus resources on high-impact, future-facing features like **weather-integrated planning** and event coordination.
* **Resource Constraints**: Limited weather forecasts to a 3-day window to remain within API free-tier limitations while maintaining core planning functionality.

---

### 2. 🚁 Kolibri AeroTech: Holonomic Quadcopter
The team designed and engineered a high-concurrency ground station and data pipeline for a search and rescue drone to overcome sensor-blindness inherent in traditional flight mechanics. This project involved architecting a multi-layered software stack using **Next.js** for real-time **LiDAR, camera, and telemetry** visualization, a **Python** backend for persistent telemetry storage, and **ROS 2** nodes on a **Raspberry Pi 5** for edge sensor processing. We optimized a low-latency video pipeline using **WebRTC** and **FFmpeg** and implemented a **push-based architecture** to maximize performance on a resource-constrained **DigitalOcean VPS**. The infrastructure leverages **MAVLink** for bidirectional flight control and utilizes secure **reverse proxies** and custom **IPv4 routing** to bridge local hardware access points with public cloud services.

---

