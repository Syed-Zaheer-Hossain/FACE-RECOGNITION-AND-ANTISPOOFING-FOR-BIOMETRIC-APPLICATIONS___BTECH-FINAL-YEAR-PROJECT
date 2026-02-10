# Face Recognition and Anti-Spoofing for Biometric Applications  
### B.Tech Final Year Project

This repository contains the implementation of a **Face Recognition and Anti-Spoofing System** designed for secure biometric authentication.  
The system integrates **face recognition** with **liveness (anti-spoofing) detection** to prevent presentation attacks such as printed photos, mobile screen replays, and video attacks.

This work is supported by a **self-made dataset** and has been **published as a research paper**.

---

## 📌 Project Highlights

- Real-time face recognition  
- Anti-spoofing (liveness detection)  
- Self-made dataset (real + spoof samples)  
- Integrated GUI application  
- Published research work (Springer)  

---

## 📚 Published Research Paper

**FRAD: A Face Recognition and Anti-spoofing Database for Biometric Applications**

- **DOI:** https://doi.org/10.1007/978-981-96-7614-9_32  
- **Publisher:** Springer (Lecture Notes in Computer Science)  
- **Authors:**  
  Saiyed Umer, Surjit Mandal, Syed Zaheer Hossain, Anirban Guha, Ranjeet Kumar Rout  

If you use this project or dataset for academic or research purposes, please cite this paper.

---

## 🚀 Project Overview

Biometric systems based on facial recognition are widely used in access control, attendance systems, and identity verification.  
However, traditional face recognition systems are vulnerable to **spoofing attacks** such as:

- Printed photographs  
- Mobile/laptop screen replays  
- Video-based attacks  

This project addresses these challenges by combining:
- **Face Recognition** for identity verification  
- **Anti-Spoofing Detection** to ensure the presence of a live human subject  

Authentication is granted **only when both modules succeed**, making the system robust and secure.

---

## 🧠 Key Features

- Face detection and preprocessing  
- Facial feature extraction  
- Anti-spoofing (liveness) classification  
- Real-time webcam input  
- GUI-based user interaction  
- Modular and extensible codebase  

---

```
FACE-RECOGNITION-AND-ANTISPOOFING-FOR-BIOMETRIC-APPLICATIONS
│
├── Dataset/
│   ├── Real/
│   │   ├── Images/            # Live face images captured from real users
│   │   └── Videos/            # Live face video samples
│   │
│   ├── Spoof/
│   │   ├── Printed_Photos/    # Spoof attacks using printed face images
│   │   ├── Screen_Replay/     # Spoof attacks using mobile/laptop screens
│   │   └── Video_Attacks/     # Replayed video-based spoof samples
│   │
│   └── README.md              # Dataset description & acquisition details
│
├── AntiSpoofing/
│   ├── preprocessing.py       # Preprocessing for spoof detection
│   ├── feature_extraction.py  # Liveness / texture feature extraction
│   ├── train_model.py         # Anti-spoofing model training
│   ├── test_model.py          # Model evaluation & testing
│   └── utils.py               # Helper functions
│
├── FaceRecognition/
│   ├── face_detection.py      # Face detection logic
│   ├── face_alignment.py      # Face normalization & alignment
│   ├── feature_extractor.py   # Facial feature extraction
│   ├── classifier.py          # Identity classification
│   └── recognition_pipeline.py# End-to-end recognition workflow
│
├── GUI_Interface/
│   ├── main_gui.py             # Tkinter-based GUI entry point
│   ├── webcam_stream.py       # Real-time webcam feed
│   ├── auth_logic.py          # Combined recognition + anti-spoof logic
│   └── assets/                # Icons, images, UI resources
│
├── requirements.txt           # Python dependencies
├── README.md                  # Project documentation
└── LICENSE                    # MIT License
```

---

## 🗂️ Folder Description Summary

| Folder / File | Description |
|--------------|-------------|
| **Dataset/** | Self-made dataset with real and spoof face samples used in the published paper |
| **AntiSpoofing/** | Liveness detection and spoof prevention modules |
| **FaceRecognition/** | Face detection, feature extraction, and identity recognition |
| **GUI_Interface/** | Integrated real-time GUI application |
| **requirements.txt** | Required Python dependencies |
| **README.md** | Project documentation |
| **LICENSE** | MIT License |

---

## 📊 Dataset Description

- The dataset is **self-created** for this project  
- Contains both **real (live)** and **spoof (fake)** samples  
- Spoof samples include:
  - Printed photographs  
  - Screen replay attacks  
  - Video-based attacks  
- Used for training and evaluating both face recognition and anti-spoofing models  

> Dataset availability can be added here (Google Drive / Zenodo) if required.

---

## 🛠️ Installation & Setup

### 1️⃣ Clone the Repository
```bash
git clone https://github.com/Syed-Zaheer-Hossain/FACE-RECOGNITION-AND-ANTISPOOFING-FOR-BIOMETRIC-APPLICATIONS-BTECH-FINAL-YEAR-PROJECT-.git
cd FACE-RECOGNITION-AND-ANTISPOOFING-FOR-BIOMETRIC-APPLICATIONS-BTECH-FINAL-YEAR-PROJECT-
```

### 2️⃣ Create Virtual Environment (Optional)
```bash
python -m venv venv
source venv/bin/activate        # Linux / macOS
venv\Scripts\activate           # Windows
```

### 3️⃣ Install Dependencies
```bash
pip install -r requirements.txt
```

---

## ▶️ Running the Application

```bash
python main.py
```

---

## 🔍 System Workflow

1. Capture face input using webcam  
2. Detect and preprocess face region  
3. Perform face recognition  
4. Apply anti-spoofing (liveness detection)  
5. Authenticate user only if both checks pass  

---

## 🧪 Future Enhancements

- Deep learning-based anti-spoofing models  
- Integration with FaceNet / ArcFace  
- Mobile or embedded deployment  
- Encrypted biometric storage  
- Cloud-based authentication  

---

## 📜 License

This project is licensed under the MIT License.  
See the LICENSE file for more details.

---

## 🤝 Acknowledgements

- Springer LNCS  
- Academic mentors and faculty  
- Contributors and reviewers  
