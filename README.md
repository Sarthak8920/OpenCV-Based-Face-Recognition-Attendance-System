# OpenCV-Based Face Recognition Attendance System

A Python application that uses OpenCV to perform face recognition and automate attendance marking. Users can register new students, login, and the system tracks attendance in a CSV file.

---

## Table of Contents
- [Features](#features)  
- [Prerequisites](#prerequisites)  
- [Installation](#installation)  
- [Usage](#usage)  
- [File Structure](#file-structure)  
- [Contributing](#contributing)  
- [License](#license)  
- [Contact](#contact)  

---

## Features
- Register new students with their images and details  
- Face recognition using OpenCV's Haar cascade  
- Automatic attendance logging to `attendance.csv`  
- Login system for users  
- GUI dialogs for adding users, registrations, and status display  

---

## Prerequisites
- Python 3.x  
- OpenCV (`cv2`)  
- Other dependencies as listed in `requirements.txt` (e.g., PyQt5, pandas, etc.)  

---

## Installation
1. Clone the repository:  
   ```bash
   git clone https://github.com/Sarthak8920/OpenCV-Based-Face-Recognition-Attendance-System.git
   cd OpenCV-Based-Face-Recognition-Attendance-System
   ```

2. (Optional) Create a virtual environment:  
   ```bash
   python3 -m venv venv
   source venv/bin/activate   # On Windows: venv\Scripts\activate
   ```

3. Install dependencies:  
   ```bash
   pip install -r requirements.txt
   ```

4. Make sure you have the Haar cascade file:  
   ```
   haarcascade_frontalface_default.xml
   ```

---

## Usage
1. **Register Students**  
   Run the student registration dialog to add a new student's details and capture images:  
   ```bash
   python student_registration_dialog.py
   ```

2. **Add Users / Admin**  
   For adding new users/admins:  
   ```bash
   python add_user_dialog.py
   ```

3. **Login**  
   Run the login dialog to authenticate:  
   ```bash
   python login_dialog.py
   ```

4. **Main Attendance System**  
   After login, run the main application to start recognizing faces and marking attendance:  
   ```bash
   python main.py
   ```

5. Attendance records will be saved in `attendance.csv`.  

---

## File Structure
```
OpenCV-Based-Face-Recognition-Attendance-System/
├── icons/
├── add_user_dialog.py
├── attendance.csv
├── credentials.json
├── haarcascade_frontalface_default.xml
├── login_dialog.py
├── main.py
├── remember.me
├── requirements.txt
├── status_widget.py
├── student_registration_dialog.py
├── students.csv
└── README.md
```

- **icons/** — GUI icons and image assets  
- **credentials.json** — Stores login credentials  
- **students.csv** — Student details (name, ID, etc.)  
- **attendance.csv** — Attendance logs (date, time, student details)  
- **status_widget.py** — Displays status messages in GUI  
- **remember.me** — Stores user login sessions  
- **haarcascade_frontalface_default.xml** — Haar cascade classifier for face detection  

---

## Contributing
Contributions are welcome!  
- Fix bugs  
- Add new features (e.g., advanced face recognition with deep learning, improved UI)  
- Enhance documentation  

To contribute:  
1. Fork the repository  
2. Create a new branch  
3. Commit your changes  
4. Open a pull request  

---

## License
This project is licensed under the **MIT License**.  

---

## Contact
- **Author**: Sarthak (GitHub: [@Sarthak8920](https://github.com/Sarthak8920))  
- Email: *sharthakkumar003@gmail.com*  
