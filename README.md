# AI-Based Early Childhood Glaucoma Risk Screening System

An AI-powered web application that screens for early signs of glaucoma risk in children using eye image analysis. The system combines a classical **Cup-to-Disc Ratio (CDR)** calculation with a **CNN-based deep learning model** to deliver fast, accessible, and clinically informative screening reports.

---

## 🩺 Overview

Glaucoma is often called the "silent thief of sight" — early detection is critical, especially in children where symptoms are rarely noticed until vision loss has already begun. This project provides a low-cost, accessible pre-screening tool that analyzes eye images (via webcam or upload) and generates a detailed risk report, helping flag cases that need further ophthalmological evaluation.

---

## ✨ Key Features

- **Hybrid Risk Analysis** — Combines traditional CDR (Cup-to-Disc Ratio) measurement with a CNN classifier (~88% accuracy) for more reliable risk assessment.
- **Two Scan Modes**
  - 📷 **Webcam Scan** — Real-time eye capture and analysis
  - 🖼️ **Image Upload** — Analyze existing eye images
- **Symptom Questionnaire** — Captures clinical symptoms alongside image data for a fuller risk picture.
- **Professional Clinical Report UI** — Dark-themed, easy-to-read report layout suitable for clinical presentation.
- **Separate Report Routing** — Dedicated report generation flows for webcam vs. uploaded image scans.

---

## 🛠️ Tech Stack

| Layer | Technology |
|---|---|
| Backend | Python, Flask |
| Image Processing | OpenCV |
| Machine Learning | CNN (Convolutional Neural Network) |
| Database | MySQL |
| Frontend | HTML, CSS, JavaScript |

---

## 📐 System Architecture

1. **Image Acquisition** — Eye image captured via webcam or uploaded by user.
2. **Preprocessing** — OpenCV handles image cleanup, cropping, and normalization.
3. **CDR Calculation** — Classical image-processing pipeline computes the Cup-to-Disc Ratio.
4. **CNN Classification** — Deep learning model predicts glaucoma risk probability.
5. **Hybrid Scoring** — CDR + CNN outputs combined for final risk assessment.
6. **Symptom Correlation** — Questionnaire responses factored into the final report.
7. **Report Generation** — Clinical-style report rendered with risk level, key metrics, and recommendations.

---

## 🚀 Getting Started

### Prerequisites
- Python 3.8+
- MySQL Server
- pip

### Installation

```bash
# Clone the repository
git clone https://github.com/<your-username>/<repo-name>.git
cd <repo-name>

# Create virtual environment
python -m venv venv
source venv/bin/activate   # On Windows: venv\Scripts\activate

# Install dependencies
pip install -r requirements.txt

# Configure MySQL database
# Update DB credentials in config.py / .env

# Run the app
python app.py
```

Visit `http://localhost:5000` in your browser.

---

## 📁 Project Structure

```
├── static/                # CSS, JS, images
├── templates/              # HTML templates
├── model/                  # Trained CNN model files
├── utils/                  # CDR calculation & image processing scripts
├── app.py                  # Main Flask application
├── requirements.txt
└── README.md
```

---

## 📊 Model Performance

- **CNN Accuracy:** ~88%
- **Approach:** Hybrid (CDR + CNN)
- **Input Modes:** Webcam capture, Image upload

---

## 🔮 Future Enhancements

- Mobile app integration
- Larger, more diverse pediatric eye image dataset
- Integration with hospital EHR systems
- Multi-language report support

---

## 📄 Research

This project's methodology has been documented in a research paper submitted to IRO Journals (JIIP).

---

## 👩‍💻 Author

**Mubitha**
B.E. Computer Science Engineering, V V College of Engineering, Tirunelveli

---

## 📜 License

This project is for academic and research purposes.
