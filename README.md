# comptage-savons
Ce projet consiste à développer un système automatique permettant de détecter, suivre et compter les savons à partir d'une séquence des images issues d'une caméra mise en place au sein du convoyeur.
# 🧼 Automated Soap Inspection & Counting System (YOLOv8 + OpenCV)

An end-to-end Computer Vision pipeline designed for real-time automated soap detection, tracking, counting, and quality anomaly inspection on industrial conveyor belts. Developed for **Huileries Belhassane (H.S.B)**.

---

## 📌 Project Overview
* **Object Detection**: Fine-tuned YOLOv8 model for real-time detection of soap bars.
* **Tracking & Counting**: Virtual line-crossing logic implemented using ByteTrack / BoT-SORT algorithms.
* **Anomaly Detection**: Real-time classification of packaging flaws (torn packaging, misalignment, missing wrapper).
* **Metrics & Reporting**: Automated generation of performance metrics ($T_d$ Detection Rate, $P_c$ Counting Accuracy) and output CSV reports.

---

## 🛠️ Tech Stack
* **Language**: Python 3.x
* **Frameworks**: Ultralytics YOLOv8, OpenCV, Pandas, NumPy
* **Environment**: Jupyter Notebook / Anaconda

---

## 📊 Performance Metrics
The system was evaluated under various confidence thresholds:

| Metric | Formula | Test 1 Score |
| :--- | :--- | :--- |
| **Detection Rate ($T_d$)** | $\frac{N_{\text{correct detections}}}{N_{\text{real soaps}}} \times 100$ | **100%** |
| **Counting Precision ($P_c$)** | $\frac{N_{\text{correctly counted}}}{N_{\text{real soaps}}} \times 100$ | **100%** |

---

## 🚀 How to Run

1. **Clone the repository:**
   ```bash
   git clone [https://github.com/SOKAINA-PY/comptage-savons.git](https://github.com/SOKAINA-PY/comptage-savons.git)
   cd comptage-savons
