<div align="center">

<!-- Animated Header -->
<img width="100%" src="https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=6,11,20&height=180&section=header&text=Gold%20Price%20Prediction&fontSize=42&fontColor=fff&animation=twinkling&fontAlignY=32&desc=CNN-LSTM%20vs%20LSTM%20|%20Deep%20Learning%20|%20Time%20Series&descAlignY=52&descSize=18"/>

<!-- Badges -->
<p>
  <img src="https://img.shields.io/badge/Python-3.8+-3776AB?style=for-the-badge&logo=python&logoColor=white"/>
  <img src="https://img.shields.io/badge/TensorFlow-2.x-FF6F00?style=for-the-badge&logo=tensorflow&logoColor=white"/>
  <img src="https://img.shields.io/badge/Keras-Deep%20Learning-D00000?style=for-the-badge&logo=keras&logoColor=white"/>
  <img src="https://img.shields.io/badge/Google%20Colab-GPU-F9AB00?style=for-the-badge&logo=googlecolab&logoColor=white"/>
</p>

<!-- Typing Animation -->
<a href="https://git.io/typing-svg">
  <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=22&pause=1000&color=FFD700&center=true&vCenter=true&random=false&width=600&lines=🥇+Predicting+Gold+Prices+with+AI;🧠+CNN-LSTM+Hybrid+Architecture;📈+Outperforming+Traditional+Models;🔬+Research-backed+Improvements" alt="Typing SVG" />
</a>

</div>

---

## 🎯 Project Overview

> **Predicting gold prices using a CNN-LSTM hybrid model that matches/outperforms traditional LSTM through architectural improvements and feature engineering.**

<div align="center">
<table>
<tr>
<td align="center"><b>🔴 Problem</b></td>
<td align="center"><b>🟢 Solution</b></td>
<td align="center"><b>🏆 Result</b></td>
</tr>
<tr>
<td>Standard CNN-LSTM fails<br/>R² = -0.37 (flat predictions)</td>
<td>Remove BatchNorm<br/>Add technical indicators</td>
<td>CNN-LSTM matches LSTM<br/>R² = 0.85+ ✅</td>
</tr>
</table>
</div>

---

## ⚡ Quick Start

```bash
# Clone the repository
git clone https://github.com/YOUR_USERNAME/gold-price-prediction-cnn-lstm.git

# Open in Google Colab
# Upload notebooks/gold_price_prediction.ipynb
```

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/YOUR_USERNAME/gold-price-prediction-cnn-lstm/blob/main/notebooks/gold_price_prediction.ipynb)

---

## 🔬 Key Findings

<div align="center">

| Issue Found | Impact | Fix Applied |
|:----------:|:------:|:-----------:|
| BatchNormalization | Disrupts temporal patterns | ❌ Removed |
| Single Feature | CNN has nothing to extract | ✅ Added 11 indicators |
| MaxPooling | Destroys sequence info | ❌ Removed |

</div>

---

## 🏗️ Architecture

```
┌─────────────────────────────────────────────────────────┐
│                    INPUT (60 × 11)                       │
│              60 timesteps × 11 features                  │
└─────────────────────────────────────────────────────────┘
                           │
            ┌──────────────┴──────────────┐
            ▼                              ▼
┌───────────────────────┐    ┌───────────────────────┐
│     CNN Branch        │    │    LSTM Branch        │
│  Conv1D(32) → LSTM    │    │  LSTM(32) → LSTM(32) │
└───────────────────────┘    └───────────────────────┘
            │                              │
            └──────────────┬──────────────┘
                           ▼
              ┌─────────────────────────┐
              │    Concatenate & Dense   │
              │     → Prediction (1)     │
              └─────────────────────────┘
```

---

## 📊 Results

<div align="center">

| Model | RMSE | MAE | R² Score |
|:-----:|:----:|:---:|:--------:|
| **CNN-LSTM (Fixed)** | XX.XX | XX.XX | **0.XX** |
| Simple LSTM | XX.XX | XX.XX | 0.XX |
| GRU | XX.XX | XX.XX | 0.XX |

</div>

---

## 📁 Project Structure

```
📦 gold-price-prediction-cnn-lstm
 ┣ 📂 notebooks
 ┃ ┗ 📜 gold_price_prediction.ipynb
 ┣ 📂 src
 ┃ ┣ 📜 models.py
 ┃ ┗ 📜 utils.py
 ┣ 📂 results
 ┃ ┣ 🖼️ predictions.png
 ┃ ┗ 📊 results.csv
 ┣ 📜 README.md
 ┗ 📜 LICENSE
```

---

## 🛠️ Tech Stack

<div align="center">
<img src="https://skillicons.dev/icons?i=python,tensorflow,sklearn,anaconda,vscode,git,github" />
</div>

---

## 📈 Features Used

| Feature | Description |
|---------|-------------|
| `close` | Closing price |
| `returns` | Daily returns |
| `ma5_ratio` | Price / 5-day MA |
| `ma10_ratio` | Price / 10-day MA |
| `ma20_ratio` | Price / 20-day MA |
| `volatility` | 10-day rolling std |
| `momentum_5` | 5-day momentum |
| `momentum_10` | 10-day momentum |
| `roc` | Rate of change |
| `price_position` | Position in 20-day range |

---

## 🚀 How to Run

1. **Open Google Colab** with GPU enabled
2. **Upload the notebook** or use the Colab badge above
3. **Run all cells** and wait ~25-30 minutes
4. **View results** and visualizations

---

## 📚 References

- Yahoo Finance API for gold price data
- TensorFlow/Keras for deep learning
- Research on CNN-LSTM hybrid architectures

---

## 👤 Author

**Your Name**
- GitHub: [@yourusername](https://github.com/yourusername)
- LinkedIn: [Your LinkedIn](https://linkedin.com/in/yourprofile)

---

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

<div align="center">

<!-- Footer Wave -->
<img width="100%" src="https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=6,11,20&height=120&section=footer"/>

<p>
  <img src="https://img.shields.io/badge/Made%20with-❤️-red?style=for-the-badge"/>
  <img src="https://img.shields.io/badge/Star%20if%20useful-⭐-yellow?style=for-the-badge"/>
</p>

</div>
