# 📦 Objectron Streamlit App (MediaPipe)

A robust **Streamlit** interface for **MediaPipe Objectron**, enabling real-time 3D object detection and pose estimation. This application detects 3D bounding boxes around common objects and extracts spatial data suitable for robotics, AR, and research.

---
## Demo Imgaes

![demo](https://github.com/Tanmay1112004/3D-Object-Detection--3d-bounding-boxes--with-mediapipe-objectron/blob/main/screenshots/Screenshot%202025-09-07%20184454.png)

![demo](https://github.com/Tanmay1112004/3D-Object-Detection--3d-bounding-boxes--with-mediapipe-objectron/blob/main/screenshots/Screenshot%202025-09-07%20185120.png)

![demo](https://github.com/Tanmay1112004/3D-Object-Detection--3d-bounding-boxes--with-mediapipe-objectron/blob/main/screenshots/Screenshot%202025-09-07%20185227.png)

![demo](https://github.com/Tanmay1112004/3D-Object-Detection--3d-bounding-boxes--with-mediapipe-objectron/blob/main/screenshots/Screenshot%202025-09-07%20185135.png)

---

## 🚀 Key Features

* **3D Detection:** Supports **Cup, Chair, Shoe, and Camera** models.
* **Spatial Data:** Visualizes rotation matrices and translation vectors in real-time.
* **Smart Visualization:** High-contrast colored 3D landmarks designed for visibility against any background.
* **Dual Input:** Process images via **Direct URL** or **Local File Upload**.
* **Data Export:** One-click download of pose estimation data as a **CSV** file.
* **Optimized Performance:** Built-in auto-resize toggle to handle high-resolution images efficiently.

---

## ⚡ Quick Start: GitHub Codespaces

The fastest way to run this project is via **GitHub Codespaces**, which comes pre-configured with all necessary system dependencies (like `libGL`).

1. **Fork** this repository.
2. Click the **Code** button → **Codespaces** → **Create codespace on main**.
3. Once the environment is ready, run the following in the terminal:
```bash
streamlit run streamlit_app.py --server.port 8501 --server.address 0.0.0.0

```


4. Click **Open in Browser** when the port forwarding notification appears.

---

## 🖥️ Local Installation

If you prefer to run the application locally, follow these steps:

### Prerequisites

* **Python 3.11**
* A virtual environment manager (`venv` or `conda`)

### Setup

```bash
# 1. Clone the repository
git clone <your-repo-url>
cd <repo-name>

# 2. Create and activate a virtual environment
python -m venv .venv
source .venv/bin/activate  # Windows: .venv\Scripts\activate

# 3. Install dependencies
pip install -r requirements.txt

# 4. Launch the application
streamlit run streamlit_app.py

```

---

## 📂 Project Structure

```bash
📂 repo-root
 ┣ 📂 .devcontainer    # Pre-configured environment for Codespaces
 ┃ ┣ 📜 Dockerfile     # Installs system-level dependencies (libGL, etc.)
 ┃ ┗ 📜 devcontainer.json
 ┣ 📜 streamlit_app.py # Core application logic
 ┣ 📜 requirements.txt # Python package list
 ┗ 📜 README.md        # Documentation

```

---

## 🛠️ Troubleshooting

| Issue | Solution |
| --- | --- |
| **`libGL.so.1` Not Found** | Run: `sudo apt-get update && sudo apt-get install -y libgl1 libglib2.0-0` |
| **Slow Inference** | Enable the **Auto-resize** feature in the sidebar (Set `max_dim` to ~800). |
| **No Objects Detected** | Ensure the object is well-lit and matches the selected category (e.g., don't use 'Shoe' for a 'Cup'). |

---

## 📊 Output Data Format

The application generates a CSV containing the following spatial coordinates:

* **2D Points:** Image-space landmarks (x, y).
* **3D Points:** Camera-coordinate space landmarks (x, y, z).
* **Pose:** 3x3 Rotation Matrix and 3x1 Translation Vector.

---

## 📄 License

Distributed under the **MIT License**. See `LICENSE` for more information.

---
