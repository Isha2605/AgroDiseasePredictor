# Agro Disease Predictor

> A lightweight web application that helps farmers identify crop diseases by selecting observable symptoms — **no image upload required**, works on slow connections and low-end devices common in rural settings.

![Python](https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white)
![Flask](https://img.shields.io/badge/Flask-000000?style=flat&logo=flask&logoColor=white)
![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=flat&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=flat&logo=css3&logoColor=white)
![License](https://img.shields.io/badge/license-MIT-green)

<!-- Replace with a screenshot: ![Screenshot](assets/screenshot.png) -->

## 🎯 Problem

Image-based crop-disease classifiers dominate the research literature, but they assume a smartphone camera, good lighting, and a stable internet connection — conditions many smallholder farmers don't have. A symptom-checklist approach works on feature phones and low-bandwidth links.

## 💡 Solution

A web app where the farmer selects observable symptoms (leaf spots, wilting, discoloration, pest presence, growth stage) and receives:

1. The most likely disease(s) given the selected symptoms
2. Confidence level per prediction
3. Recommended first-line treatment and escalation path

## 🛠️ Tech Stack

| Layer | Tools |
|---|---|
| Backend | Python, Flask |
| Frontend | HTML5, CSS3 (minimal — no heavy JS) |
| Data | Symptom → disease knowledge base (curated) |

## 🚀 Getting Started

```bash
git clone https://github.com/Isha2605/Agro-Disease-Predictor.git
cd Agro-Disease-Predictor
pip install -r requirements.txt
python app.py
```

Open `http://localhost:5000`.

## 📁 Project Structure

```
├── app.py              # Flask entrypoint + routing
├── templates/          # HTML pages
│   ├── index.html      # Symptom selection form
│   └── result.html     # Disease + treatment output
├── static/
│   └── style.css
├── data/
│   └── diseases.json   # Symptom → disease knowledge base
├── requirements.txt
└── README.md
```

## 🌾 Supported Crops & Diseases

| Crop | Diseases covered |
|---|---|
| Wheat | Rust, powdery mildew, Septoria leaf blotch |
| Rice  | Blast, bacterial blight, sheath blight |
| Cotton | Bollworm, leaf curl, wilt |
| Tomato | Early blight, late blight, mosaic virus |

*(Extend by editing `data/diseases.json`.)*

## 🔮 Future Work

- [ ] Add a simple Naive Bayes model trained on symptom-disease co-occurrence
- [ ] Multilingual UI (Hindi, Marathi, Telugu)
- [ ] SMS-based interface for feature phones
- [ ] Offline PWA for fields without signal

## 📬 Contact

**Isha Narkhede** · [Portfolio](https://isha-n-portfolio.netlify.app/) · [LinkedIn](https://linkedin.com/in/isha-narkhede) · ishajayant207@gmail.com

## 📝 License

MIT — see [LICENSE](LICENSE).
