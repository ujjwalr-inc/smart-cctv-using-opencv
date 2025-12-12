# 🔐 Smart CCTV Using Computer Vision

A smart CCTV system that uses computer vision, motion detection, and face recognition to monitor environments, detect intrusions, track movement, and record suspicious activities automatically.


---

## 🧩 Features

### 🎯 Motion Detection
- Detects motion using frame differencing (`find_motion.py`, `motion.py`)
- Highlights moving objects
- Triggers recordings when activity is detected

### 👁️ Face Detection & Identification
- Uses OpenCV Haar Cascade (`haarcascade_frontalface_default.xml`)
- Identifies known individuals
- Saves unknown faces for review

### 🎥 Automatic Recording
- Records only when motion is present
- Saves videos in `/recordings/`

### 🚶‍♂️🚶‍♀️ In/Out Person Tracking
- Tracks entry & exit (`in_out.py`)
- Saves images in:
	-`persons/in/`
	-`persons/out/`

### 🕵️ Suspicious Activity Detection
- Detects anomalies / spot differences (`spot_diff.py`)
- Saves extracted frames in /stolen/

### 📊 Analytics & Graph Tracing
Visualizes activity using graph tracing.py

---

## 📁 Project Structure
~~~
Smart CCTV Using Computer Vision/
│
├── icons/                        
├── recordings/                  
├── stolen/                      
├── persons/
│   ├── in/
│   └── out/
├── main.py                       
├── identify.py                   
├── find_motion.py                
├── motion.py                     
├── spot_diff.py                  
├── record.py                     
├── in_out.py                     
├── graph tracing.py              
├── haarcascade_frontalface_default.xml         
└── requirements.txt
~~~

---

## ⚙️ Installation

1️⃣Create and activate virtual environment
```bash
python -m venv .venv
.venv\Scripts\activate
```
2️⃣ Install Dependencies
```bash
pip install -r requirements.txt
```

---

## ▶️ Usage

### 🚀 Start the CCTV System
```bash
python main.py
```
### 🔬 Run Individual Modules

#### Face Detection
```bash
python identify.py
```
#### Motion Detection
```bash
python find_motion.py
```
#### In/Out Tracking
```bash
python in_out.py
```
---

## 🛠️ Technologies Used

🐍 **Python**  
👁️ **OpenCV**  
🧱 **Haar Cascade Classifiers**  

---

## 📜 License
This project is open-source under the **MIT License**.

---
