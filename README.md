# EDukaan – AI-Powered Multilingual Product Listing Assistant

Welcome to the official repository for **Team TechSpectra's** iDEA Hackathon project, led by **Harish Lukare**. Our innovative solution empowers small and medium Indian sellers by automating product listings using AI/ML and voice inputs in **any Indian language**.

## 🚀 Problem Statement

Many sellers, especially in rural or semi-urban areas, face challenges listing products online due to language barriers, lack of technical expertise, and time-consuming manual entry. Our solution bridges this digital divide by enabling sellers to describe their products **verbally in their native language**, and the app will handle everything else.

---

## 💡 Solution Overview

We developed a multilingual Android application integrated with an AI-powered backend to:
1. **Accept product descriptions via speech or video.**
2. **Convert speech to text** (any Indian language to English).
3. **Extract structured product information** (title, category, price, features).
4. **Generate ready-to-use product listings**, including uploading images to the cloud.

---

## 🧠 Tech Stack

### Frontend (Mobile App)
- **React Native** (cross-platform)
- Camera & microphone integration
- File/image picker & Cloudinary integration

### Backend (AI/ML)
- **Python (Flask API)** for AI processing
- **spaCy** & **transformers** for NLP
- **SpeechRecognition** + **Google/Whisper API** for multilingual speech-to-text
- **Price extraction** using regex/NLP patterns
- **Translation** with `googletrans` or Indic NLP library

---

## 📦 Features

- 🎙️ **Voice Input** in any Indian language  
- 🌐 **Automatic Translation** to English  
- 🧾 **Smart Extraction** of product name, description, and price  
- 🏷️ **Category Mapping** based on keywords  
- ☁️ **Cloud Upload** of product images via Cloudinary  
- 📃 **Auto-generated product listing format**  
- 🔁 Option to review, edit, and confirm listing

---

## 🔍 Sample Use Case

> A rural seller records a video saying in Hindi:  
> "यह एक हाथ से बुना हुआ दुपट्टा है, कीमत 350 रुपये है।"  
>  
> Our app converts this to:  
> "**This is a handwoven dupatta, price is ₹350.**"  
> Then it extracts:
> - **Title**: Handwoven Dupatta  
> - **Price**: ₹350  
> - **Category**: Clothing > Women > Dupattas  
> - **Description**: Handcrafted traditional dupatta perfect for festive occasions.

---

## 📊 AI/ML Pipeline

1. **Audio Processing** → Language Detection  
2. **Speech-to-Text** (Whisper API / Google STT)  
3. **Translation** (Indic NLP / Google Translate API)  
4. **NLP Parsing** → spaCy-based custom NER & rule-based extraction  
5. **Category Mapping** using similarity scoring & keyword matching  
6. **Output JSON** sent to the mobile app for UI display and listing

---

## 🛠️ Setup Instructions

### Backend
```bash
git clone https://github.com/hlukare/EDukaan-a-Customer-Seller-Application.git
cd EDukaan-a-Customer-Seller-Application
pip install -r requirements.txt
python app.py
```

## Other files will be uploaded soon.
