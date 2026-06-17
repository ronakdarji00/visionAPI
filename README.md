# Vision API — Free AI Background Remover, Face Verification & Detection API

> ⚡ **Remove image backgrounds, verify faces, and analyze facial attributes — all in one free API.**

[![Website](https://img.shields.io/badge/Website-bgremoverproai.store-blue)](https://bgremoverproai.store)
[![Free Tier](https://img.shields.io/badge/Free%20Tier-100%20Credits-green)](https://bgremoverproai.store/pricing)
[![API Docs](https://img.shields.io/badge/API%20Docs-Available-orange)](https://bgremoverproai.store/docs)

---

## 🚀 What is Vision API?

**Vision API** is a free, fast, and developer-friendly image processing API platform powered by state-of-the-art AI models.

Built for developers, e-commerce sellers, content creators, and digital marketers who need:
- **Background removal** with hair-level precision
- **Face verification** with liveness detection
- **Face analysis** (age, gender, expression, landmarks)

---

## ✨ Core Features

### 1. 🖼️ AI Background Removal
- **Models:** BiRefNet + BRIA RMBG
- **Output:** Transparent PNG with hair-level edge precision
- **Modes:** Advanced, Standard, Person
- **Speed:** ~1-2 seconds per image
- **Free quota:** ~20 removals with signup

**Endpoint:** `POST /api/remove-bg`

```bash
curl -X POST https://bgremoverproai.store/api/remove-bg \
  -H "X-API-Key: YOUR_API_KEY" \
  -F "file=@photo.jpg"
```

### 2. 🔐 Face Verification API
- **Models:** RetinaFace + ArcFace
- **Features:** 1:1 matching, 1:N search, liveness detection
- **Score:** Similarity score 0.0 - 1.0
- **Use cases:** KYC, attendance, secure login

**Endpoint:** `POST /api/face/verify`

```bash
curl -X POST https://bgremoverproai.store/api/face/verify \
  -H "X-API-Key: YOUR_API_KEY" \
  -F "file1=@id_photo.jpg" \
  -F "file2=@selfie.jpg"
```

### 3. 📊 Face Analysis API
Detects and analyzes multiple faces in a single image:
- Age estimation
- Gender detection
- Expression recognition (happy, sad, angry, surprise, neutral)
- Head pose (yaw, pitch, roll)
- Eye state & mouth openness
- Smile detection
- Face shape (oval, round, square, heart, diamond, oblong)
- 106-point facial landmarks

**Endpoint:** `POST /api/face/analyze`

```bash
curl -X POST https://bgremoverproai.store/api/face/analyze \
  -H "X-API-Key: YOUR_API_KEY" \
  -F "file=@group_photo.jpg"
```

---

## 🆓 Pricing

| Tier | Credits | Price |
|------|---------|-------|
| Free (Signup) | 100 | $0 |
| Starter | 1000 | $5 |
| Pro | 5000 | $20 |
| Enterprise | 25000 | $75 |

**1 Credit ≈ 1 API call.** No hidden fees. No subscription required.

👉 [View full pricing](https://bgremoverproai.store/pricing)

---

## 🛠️ Tech Stack

- **Backend:** Python FastAPI
- **Deep Learning:** PyTorch, ONNX Runtime, CUDA (NVIDIA Tesla T4)
- **Models:** BiRefNet, BRIA RMBG, RetinaFace, ArcFace
- **Face Engine:** InsightFace
- **Deployment:** AWS EC2 g4dn.xlarge, Docker
- **Frontend:** React, Vite, Tailwind CSS
- **Payment:** Razorpay (India)

---

## 🏗️ Architecture

```
┌─────────────────┐     ┌──────────────┐     ┌─────────────────┐
│   React Client  │────▶│  FastAPI     │────▶│  AI Models      │
│   (Vite + TW)   │     │  (Uvicorn)   │     │  (PyTorch/CUDA) │
└─────────────────┘     └──────────────┘     └─────────────────┘
                               │
                               ▼
                        ┌──────────────┐
                        │  MongoDB     │
                        │  Atlas       │
                        └──────────────┘
```

---

## 📝 API Documentation

Full docs with code examples in cURL, JavaScript, Python, and PHP:

👉 [https://bgremoverproai.store/docs](https://bgremoverproai.store/docs)

---

## 🔗 Useful Links

| Resource | URL |
|----------|-----|
| 🌐 Website | [bgremoverproai.store](https://bgremoverproai.store) |
| 🖼️ Background Remover | [bgremoverproai.store/background-remover](https://bgremoverproai.store/background-remover) |
| 🔐 Face Verification | [bgremoverproai.store/face-verification](https://bgremoverproai.store/face-verification) |
| 📊 Face Analysis | [bgremoverproai.store/face-analysis](https://bgremoverproai.store/face-analysis) |
| 💰 Pricing | [bgremoverproai.store/pricing](https://bgremoverproai.store/pricing) |
| 📖 API Docs | [bgremoverproai.store/docs](https://bgremoverproai.store/docs) |
| 📧 Contact | hackersmeet.official@gmail.com |

---

## 🔒 Privacy & Security

- Images are processed **in memory** and immediately discarded
- No image storage, training, or sharing without explicit consent
- API key authentication on all endpoints
- HTTPS/TLS encryption

---

## 🌟 Why Vision API?

| Feature | Vision API | Others |
|---------|-----------|--------|
| Free tier with real credits | ✅ 100 credits | Usually none |
| Hair-level BG removal | ✅ BiRefNet + BRIA | Basic cutouts |
| Liveness detection | ✅ Included | Often paid extra |
| Multi-face analysis | ✅ Up to 20 faces | Usually single |
| No image storage | ✅ Privacy-first | Often stores data |
| Indian payment support | ✅ Razorpay | Mostly Stripe |

---

## 🤝 Contributing

We welcome feedback and feature requests!

📧 **Email:** hackersmeet.official@gmail.com

---

## 📄 License

All rights reserved © Vision API / Hackersmeet

---

> Built with ❤️ by [Hackersmeet](https://bgremoverproai.store)
