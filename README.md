# MajiSmart 💧 - AI Water Leak Detection for Mwanza

> Built for PayPal AI Hackathon 2026 | Saving water, empowering communities in Tanzania

### 🎯 Problem
40% of clean water in Mwanza is lost through undetected leaks in homes. Families pay high bills, MWAUWASA loses revenue.

### 💡 Solution
MajiSmart uses AI on smartphones to detect leaks from photos & sounds, then uses PayPal to fund local plumbers.

### 🚀 PayPal Integration (Required)

1. **PayPal Checkout SDK (JS SDK)** - Community crowdfunding. Anyone worldwide can donate $5-$100 to fix a verified leak. 
   `paypal.Buttons()` rendered in Next.js frontend. Webhook: `PAYMENT.CAPTURE.COMPLETED`

2. **PayPal Payouts API (REST v1)** - Auto-disburses 90% of donations directly to local fundis (plumbers) PayPal accounts.
   Endpoint: `POST /v1/payments/payouts` - Transparent & instant.

3. **PayPal Webhooks** - Real-time tracking. Updates donation progress & triggers payout status.

4. **PayPal QR Donate** - For offline posters in Swahili markets.

### 🤖 AI Integration (Required)

1. **TensorFlow Lite - Image Model:** Custom CNN trained on 2,500+ images of damp walls, mold, pipe rust. 92% accuracy, 4.2MB, runs offline on phone.

2. **TensorFlow Audio - Sound Model:** Uses Librosa to convert 3-sec drip sound to mel-spectrogram, classifies leak severity (low/medium/high).

3. **OpenAI GPT-3.5:** Swahili/English chatbot explains leak cause & prevention.

### 🛠️ Tech Stack
Next.js 14, TensorFlow.js, Python (training), PayPal SDKs, Vercel

### 👤 Team
Individual: mapulimapuli782-cloud from Mwanza, Tanzania

### 🔗 Links
Devpost: https://devpost.com/software/majismart
Demo: https://maji-smart.vercel.app (coming soon)

Built with love for Mwanza 
