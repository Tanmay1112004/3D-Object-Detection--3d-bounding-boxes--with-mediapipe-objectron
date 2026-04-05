# 📦 Objectron 3D Detection App (MediaPipe + Streamlit)

> **Real-time 3D Object Detection & Pose Estimation — Built for AR, Robotics, and Vision Systems**

An end-to-end **computer vision application** that leverages **MediaPipe Objectron** to detect objects in 3D space and estimate their **pose (rotation + translation)** — wrapped inside a clean, interactive **Streamlit UI**.

---

## 🎥 Demo Preview

![demo](https://github.com/Tanmay1112004/3D-Object-Detection--3d-bounding-boxes--with-mediapipe-objectron/blob/main/screenshots/Screenshot%202025-09-07%20184454.png)

![demo](https://github.com/Tanmay1112004/3D-Object-Detection--3d-bounding-boxes--with-mediapipe-objectron/blob/main/screenshots/Screenshot%202025-09-07%20185120.png)

![demo](https://github.com/Tanmay1112004/3D-Object-Detection--3d-bounding-boxes--with-mediapipe-objectron/blob/main/screenshots/Screenshot%202025-09-07%20185227.png)

![demo](https://github.com/Tanmay1112004/3D-Object-Detection--3d-bounding-boxes--with-mediapipe-objectron/blob/main/screenshots/Screenshot%202025-09-07%20185135.png)

---

## 🚀 What This Project Does

Upload an image or provide a URL →
👉 Detects real-world objects (Cup, Chair, Shoe, Camera)
👉 Draws **3D bounding boxes + landmarks**
👉 Outputs **precise spatial data** (rotation + translation)
👉 Lets you **download pose data as CSV**

This is not just detection — it’s **understanding objects in 3D space**.

---

## 🧠 Core Capabilities

### 🎯 3D Object Detection

* Detects real-world objects using **MediaPipe Objectron**
* Generates **3D bounding boxes**
* Tracks object orientation in space

### 📐 Pose Estimation

* Extracts:

  * Rotation Matrix (3×3)
  * Translation Vector (3×1)
* Enables use cases in:

  * Robotics 🤖
  * AR/VR 🥽
  * Simulation systems 🎮

### 🖼️ Smart Visualization

* High-contrast 3D overlays
* Clear landmark plotting for better interpretability
* Works across different backgrounds

### 📥 Flexible Input

* Upload local images
* Paste image URLs
* Toggle performance settings

### 📊 Data Export

* One-click CSV download
* Structured output for further ML/analytics pipelines

---

## 🛠️ Tech Stack

| Layer               | Technology          |
| ------------------- | ------------------- |
| **Language**        | Python              |
| **Computer Vision** | MediaPipe Objectron |
| **Frontend**        | Streamlit           |
| **Data Handling**   | NumPy, Pandas       |
| **Visualization**   | OpenCV              |

---

## ⚙️ System Workflow

```
Image Input (Upload / URL)
        ↓
Preprocessing (Resize / Normalize)
        ↓
MediaPipe Objectron
        ↓
3D Detection + Pose Estimation
        ↓
Visualization (Bounding Box + Landmarks)
        ↓
CSV Export (Spatial Data)
```

---

## ⚡ Quick Start

### 🔹 Run Locally

```bash
git clone Tanmay1112004
cd <repo-name>

python -m venv .venv
source .venv/bin/activate   # Windows: .venv\Scripts\activate

pip install -r requirements.txt
streamlit run streamlit_app.py
```

---

### 🔹 Run via GitHub Codespaces (Recommended)

No setup. No dependency issues. Just run.

```bash
streamlit run streamlit_app.py --server.port 8501 --server.address 0.0.0.0
```

---

## 📂 Project Structure

```
📦 Objectron-App
 ┣ 📂 .devcontainer
 ┃ ┣ 📜 Dockerfile
 ┃ ┗ 📜 devcontainer.json
 ┣ 📜 streamlit_app.py
 ┣ 📜 requirements.txt
 ┗ 📜 README.md
```

---

## 📊 Output Format

The system generates structured spatial data:

### 🔹 2D Coordinates

* Image-space points (x, y)

### 🔹 3D Coordinates

* Camera-space points (x, y, z)

### 🔹 Pose Data

* Rotation Matrix (3×3)
* Translation Vector (3×1)

👉 Ready for:

* Robotics pipelines
* AR overlays
* Physics simulations

---

## 🎯 Real-World Use Cases

* 🤖 **Robotics Navigation & Grasping**
* 🥽 **Augmented Reality Object Placement**
* 📦 **3D Object Tracking Systems**
* 🧪 **Computer Vision Research**
* 🏭 **Industrial Automation**

---

## 🔧 Performance Optimization

| Issue           | Solution                                |
| --------------- | --------------------------------------- |
| Slow processing | Enable auto-resize (max_dim ≈ 800)      |
| No detection    | Ensure object matches selected category |
| libGL error     | Install system dependencies             |

---

## 🧪 Challenges Solved

* Handling **high-resolution images efficiently**
* Visualizing **3D data in 2D UI**
* Integrating **real-time CV models into web apps**
* Managing **pose estimation outputs cleanly**

---

## 💡 Why This Project Stands Out

This project demonstrates:

✔ Applied **3D Computer Vision**
✔ Real-world **pose estimation pipeline**
✔ End-to-end **ML + UI integration**
✔ Practical understanding of **spatial data systems**

👉 This is the kind of project that moves you from *“student” → “engineer”*.

---

## 🤝 Contributing

Pull requests are welcome. Let’s build something powerful together.

---

## 📜 License

MIT License

---

## 👨‍💻 Author

**Tanmay Kshirsagar**
💼 Data Science | ML Engineering | Computer Vision

---
