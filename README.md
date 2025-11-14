# Capti-On: AI-Based Image Caption Generator  

Capti-On is an **AI-powered caption generation system** that automatically creates **context-aware, creative, and platform-specific captions** for images.  
It allows users to upload or capture real-time images, provide short prompts, and select tone, language, and platform preferences (e.g., Amazon, Meesho, Instagram, Facebook, etc.).  

Using a **CNN–LSTM deep learning model**, Capti-On blends visual understanding with natural language generation to produce captions that are accurate, human-like, and adaptable to user needs.  

---

## 🚀 Features  

- 📸 **Image Upload or Capture** — Upload existing images or capture in real-time.  
- ✍️ **Prompt-Based Captioning** — Guide captions using short product descriptions or keywords.  
- 🧩 **Tone Customization** — Choose from tones such as *Luxury, Funny, Professional, or Budget-Friendly*.  
- 🌍 **Language Options** — Generate captions in multiple languages (English, Hindi, Spanish, German, French, Arabic).  
- 💼 **Platform Adaptation** — Optimize captions for platforms like Amazon, Meesho, Flipkart, Instagram, WhatsApp, etc.  
- 💬 **Chatbot Interface** — Interactive chatbot UI for generating, copying, downloading, and sharing captions.  
- ⚡ **Real-Time Generation** — Fast and accurate results using the CNN–LSTM model.  

---

## 🧩 System Architecture  

### 1. **CNN–LSTM Model Workflow**

Image Input → Image Preprocessing → CNN (InceptionV3) → Feature Vector
Text Input → Text Preprocessing → Word Embedding → Fusion Layer
Fusion Layer → LSTM → Softmax → Caption Generation
Caption Generation → User Customization Module → Final Output



---

## ⚙️ Tech Stack  

| Component | Technology |
|------------|-------------|
| **Frontend** | HTML, CSS, JavaScript (Chatbot Interface) |
| **Backend** | Flask (Python Framework) |
| **Deep Learning** | TensorFlow / Keras |
| **Model Architecture** | CNN–LSTM |
| **Pretrained Model** | InceptionV3 |
| **Libraries Used** | NumPy, Pandas, Matplotlib, Pillow, Pickle |
| **Database** | Not Applicable (Model-based system) |
| **Tools** | Jupyter Notebook, VS Code |

---

## 📊 Dataset  

The dataset consists of **thousands of labeled product or object images** with corresponding textual captions (similar to H&M product captioning data).  
Each record contains:
- **Image Data** (JPEG format)
- **Text Captions** (descriptive sentences of product attributes)  

Data is preprocessed, cleaned, tokenized, and split into training (70%), validation (20%), and testing (10%) sets.  

---

## 🧠 Model Description  

- **CNN Backbone:** Pre-trained **InceptionV3** model for extracting visual features.  
- **Text Encoder:** Word embedding layer for tokenized captions.  
- **Fusion Layer:** Combines image features and word embeddings.  
- **Sequence Decoder:** LSTM generates captions word-by-word.  
- **Output Layer:** Softmax predicts the next word in the sequence.  
- **Loss Function:** Categorical Cross-Entropy.  
- **Optimizer:** Adam.  

---

## 🧰 Installation  

### 1️⃣ Clone this repository
```bash
git clone https://github.com/yourusername/Capti-On.git
cd Capti-On

### 2️⃣ Create virtual environment and install dependencies
python -m venv venv
source venv/bin/activate  # (or venv\Scripts\activate for Windows)
pip install -r requirements.txt

