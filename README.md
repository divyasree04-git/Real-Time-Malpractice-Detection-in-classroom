# 🎓 Real-Time Malpractice Detection in Classroom

## 📌 Project Overview

**Real-Time Malpractice Detection in Classroom** is an intelligent monitoring system designed to detect suspicious student behavior and inattentiveness during examinations or classroom sessions.

The system continuously analyzes webcam video streams in real time and identifies whether a student is attentive or potentially involved in malpractice by detecting prolonged face absence or suspicious behavior.

When malpractice is suspected:

✅ Warning messages are displayed  
✅ Alert sounds are triggered  
✅ Evidence screenshots are automatically captured  
✅ Session statistics are recorded

This project helps educational institutions improve **exam integrity**, **student monitoring**, and **classroom supervision** using **Artificial Intelligence and Computer Vision**.

---

## ✨ Features

### 🔐 User Authentication System
- User Registration
- Secure Login System
- Password Hashing using Werkzeug
- Session Management

### 🎥 Real-Time Monitoring
- Live webcam integration
- Face detection using Haar Cascade Classifier
- Continuous frame analysis
- Real-time status monitoring

### 🚨 Malpractice Detection
- Detects student inattentiveness
- Identifies prolonged face absence
- Automatic malpractice warning system
- Visual red alert notifications
- Audio beep alerts

### 📸 Automatic Evidence Collection
- Captures malpractice screenshots automatically
- Stores evidence images with timestamps
- Saves inattentive behavior records

### 📊 Dashboard & Reports
- Displays captured malpractice evidence
- Session analytics
- Student attention statistics
- Monitoring history

### 🗃 Database Support
- SQLite database integration
- User credential management
- Persistent login data

---

## 🧠 Technologies Used

| Technology | Purpose |
|------------|---------|
| Python | Core programming language |
| Flask | Web framework |
| OpenCV | Computer vision and image processing |
| NumPy | Numerical operations |
| SQLite | Database management |
| HTML/CSS | Frontend UI |
| Werkzeug | Password security |

---

## 🏗 Project Architecture

```text
User Login/Register
        │
        ▼
 Flask Web Application
        │
        ▼
 Webcam Video Stream
        │
        ▼
 OpenCV Face Detection
        │
        ├───────────────► Face Detected
        │                       │
        │                       ▼
        │                Student Attentive
        │
        └───────────────► No Face Detected
                                │
                                ▼
                      Suspicious Behavior Detected
                                │
                                ▼
                      Warning + Screenshot Capture
```

---

## 📂 Project Structure

```bash
Real-Time-Malpractice-Detection-in-classroom/
│── app.py                         # Main Flask application
│── requirements.txt              # Required dependencies
│── users.db                      # SQLite database
│── static/
│   ├── style.css                 # Styling
│   └── captured_images/          # Stored malpractice images
│
│── templates/
│   ├── index.html                # Home page
│   ├── login.html                # Login page
│   ├── register.html             # Registration page
│   └── dashboard.html            # Monitoring dashboard
│
└── attention_graphs/             # Reports and analytics
```

---

## ⚙️ How It Works

### 1️⃣ User Authentication
The user logs into the system using a secure authentication mechanism.

### 2️⃣ Start Monitoring
Once logged in, the monitoring session begins through webcam access.

### 3️⃣ Face Detection
The system uses **OpenCV Haar Cascade Face Detection** to identify faces in real time.

### 4️⃣ Attention Tracking
If a face is visible:
- Student marked as **Attentive**
- Green detection box shown

If no face is visible:
- Student marked as **Not Attentive**
- Warning mechanism starts

### 5️⃣ Malpractice Alert
If inattentiveness continues for a few seconds:
- 🚨 Red malpractice warning displayed
- 🔊 Audio alert triggered
- 📸 Screenshot captured automatically

### 6️⃣ Dashboard Analysis
The dashboard displays:
- Captured malpractice screenshots
- Session history
- Monitoring insights

---

## 🛠 Installation Guide

### Step 1: Clone the Repository

```bash
git clone <your-repository-url>
cd Real-Time-Malpractice-Detection-in-classroom
```

### Step 2: Create Virtual Environment (Recommended)

#### Windows
```bash
python -m venv venv
venv\Scripts\activate
```

#### Linux / Mac
```bash
python3 -m venv venv
source venv/bin/activate
```

### Step 3: Install Dependencies

```bash
pip install -r requirements.txt
```

### Step 4: Run the Application

```bash
python app.py
```

### Step 5: Open Browser

```text
http://127.0.0.1:5000
```

---

## 📦 Required Dependencies

```txt
Flask==2.0.1
opencv-python==4.5.3.56
numpy==1.21.2
Werkzeug==2.0.1
```

Install manually:

```bash
pip install Flask opencv-python numpy Werkzeug
```

---

## 🧪 System Requirements

### Minimum Requirements
- OS: Windows 10/11, Linux, macOS
- Python: 3.x
- RAM: 4GB+
- Webcam Required
- Internet connection (optional)

---

## 📸 Screenshots

Add screenshots here for better GitHub presentation.

Example:
```md
![Login Page](screenshots/login.png)
![Dashboard](screenshots/dashboard.png)
![Detection System](screenshots/detection.png)
```

---

## 🔍 Key Functionalities

✔ Real-time face detection  
✔ Classroom attention monitoring  
✔ AI-based malpractice detection  
✔ Screenshot evidence collection  
✔ Dashboard monitoring  
✔ Secure authentication system  
✔ Session tracking

---

## 🚀 Future Enhancements

- Deep Learning-based face recognition
- Multiple student monitoring
- Eye tracking detection
- Head pose estimation
- Mobile notifications for alerts
- Cloud-based reporting system
- Teacher/Admin analytics dashboard
- Database improvement using MySQL/PostgreSQL

---

## 🎯 Use Cases

- 🏫 Online Examination Monitoring
- 🎓 Smart Classroom Systems
- 🧑‍🏫 Student Attention Tracking
- 📝 Academic Integrity Monitoring
- 🖥 Remote Proctoring Systems

---

## 🤝 Contributing

Contributions are welcome!

1. Fork the repository  
2. Create a new branch  
3. Commit changes  
4. Push to your branch  
5. Open a Pull Request

---

## 🐛 Known Limitations

- Currently optimized for single-user monitoring
- Webcam dependency required
- Basic face detection model used
- Lighting conditions may affect accuracy

---

## 📜 License

This project is developed for **educational and research purposes**.

---

## 👨‍💻 Author

**Likitha Vattikuti**

If you like this project, don’t forget to ⭐ the repository!

---

## 🌟 Support

If this project helped you, please consider:

⭐ Starring the repository  
🍴 Forking the project  
📢 Sharing it with others
