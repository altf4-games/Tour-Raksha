# 🛡️ Tour-Raksha

**Smart Tourist Safety Monitoring & Incident Response System**

> Built by **Team Big O(6)**

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Node.js](https://img.shields.io/badge/Node.js-v18+-green.svg)](https://nodejs.org/)
[![Flutter](https://img.shields.io/badge/Flutter-3.0+-blue.svg)](https://flutter.dev/)
[![Next.js](https://img.shields.io/badge/Next.js-14+-black.svg)](https://nextjs.org/)

An intelligent tourist safety ecosystem leveraging **AI**, **Blockchain**, and **Geo-Fencing** technologies to ensure traveler security, real-time monitoring, and rapid incident response.

---

## 📋 Table of Contents

- [Overview](#overview)
- [Problem Statement](#problem-statement)
- [Key Features](#key-features)
- [Tech Stack](#tech-stack)
- [Architecture](#architecture)
- [Getting Started](#getting-started)
- [Project Structure](#project-structure)
- [API Documentation](#api-documentation)
- [Contributing](#contributing)
- [Team](#team)

---

## 🌟 Overview

**Tour-Raksha** is a comprehensive digital safety platform designed to protect tourists through:

- **🆔 Blockchain-based Digital Identity**: Secure, tamper-proof tourist IDs valid for trip duration
- **📱 Mobile Safety App**: Real-time tracking, panic button, and intelligent alerts
- **🧠 AI-Powered Monitoring**: Anomaly detection for unusual behavior patterns
- **🗺️ Geo-Fencing Alerts**: Automatic warnings for high-risk zones
- **📊 Authority Dashboard**: Real-time tourist monitoring and incident management
- **🤖 ML Safety Scoring**: Predictive safety scores based on 42+ data points

---

## 🎯 Problem Statement

In regions where tourism is a key economic driver, ensuring visitor safety is paramount. Traditional policing and manual tracking methods are insufficient in remote and high-risk areas. Tour-Raksha addresses this gap by providing:

- **Real-time monitoring** and rapid response capabilities
- **Secure identity verification** for tourists
- **Predictive analytics** for risk assessment
- **Privacy-compliant tracking** with opt-in features
- **Multilingual accessibility** for diverse travelers

### Background

Tourists, especially in remote areas like the Northeast, face challenges including:

- Limited emergency response infrastructure
- Language barriers in crisis situations
- Lack of real-time safety information
- Difficulty in tracking during emergencies
- Insufficient data for preventive measures

---

## ✨ Key Features

### 🔐 Digital Tourist ID Generation Platform ✅

- **Blockchain-based identity** system (Ethereum/Polygon)
- **KYC integration** with Aadhaar/Passport verification
- **Trip itinerary** and emergency contact storage
- **Time-bound validity** matching visit duration
- **Tamper-proof records** for audit trails

### 📱 Mobile Application for Tourists ✅

- **🚨 Panic Button**: One-tap emergency alert with live location
- **🎯 Auto Safety Score**: Dynamic scoring based on travel patterns and area sensitivity
- **🗺️ Geo-Fencing**: Instant alerts when entering restricted/high-risk zones
- **📍 Real-time Tracking**: Opt-in location sharing with family/authorities
- **🌐 Multilingual Support**: 10+ Indian languages + English
- **♿ Accessibility**: Voice/text emergency access for all users
- **📶 Offline Mode**: Critical features work without internet

### 🧠 AI-Based Anomaly Detection ✅

- **Location monitoring**: Detects sudden drop-offs or unusual movement
- **Inactivity alerts**: Flags prolonged silence or unusual patterns
- **Route deviation**: Identifies departure from planned itinerary
- **Behavioral analysis**: ML models for distress signal detection
- **Predictive alerts**: Early warning system for potential incidents

### 📊 Tourism Department & Police Dashboard ✅

- **Real-time Visualization**: Tourist clusters and movement heat maps
- **Risk Zone Mapping**: Dynamic high-risk area identification
- **Digital ID Access**: Instant tourist profile retrieval
- **Alert Management**: Centralized incident tracking
- **Automated E-FIR**: Quick missing person report generation
- **Analytics Dashboard**: Historical data and trend analysis

### 🏷️ IoT Integration (Optional) ✅

- **Smart wearables** for high-risk areas (caves, forests, mountains)
- **Continuous vitals monitoring** (heart rate, location)
- **Manual SOS trigger** on wearable devices
- **Battery alerts** and device health monitoring

### 🔒 Data Privacy & Security ✅

- **End-to-end encryption** for all communications
- **GDPR/Data Protection** law compliance
- **Blockchain security** for identity records
- **Opt-in tracking** with full user consent
- **Data retention policies** with automatic purging post-trip

---

## 🛠️ Tech Stack

### Frontend

- **🖥️ Web Dashboard**: Next.js 14, TypeScript, TailwindCSS, shadcn/ui
- **📱 Mobile App**: Flutter 3.0+, Dart
- **🗺️ Maps**: Google Maps API, Mapbox
- **📊 Visualization**: Chart.js, D3.js

### Backend

- **⚙️ API Server**: Node.js, Express.js
- **🗄️ Database**: PostgreSQL with Prisma ORM
- **🔗 Blockchain**: Solidity, Hardhat, Ethers.js
- **🔐 Authentication**: JWT, OAuth 2.0
- **📧 Communications**: Nodemailer, Twilio SMS

### AI/ML

- **🤖 Framework**: Python, scikit-learn
- **🚀 API**: FastAPI
- **📈 Models**: Linear Regression (R² 0.97+), Random Forest
- **🔍 Features**: 42+ safety indicators

### DevOps

- **☁️ Hosting**: Vercel (Frontend), Railway/Render (Backend)
- **🔄 CI/CD**: GitHub Actions
- **📦 Containerization**: Docker
- **🌐 CDN**: Cloudflare

---

## 🏗️ Architecture

```
┌─────────────────────────────────────────────────────────────┐
│                      Tourist Ecosystem                       │
├──────────────┬──────────────┬──────────────┬────────────────┤
│ Flutter App  │  Next.js Web │  IoT Devices │  ML Service    │
│ (Tourist)    │  (Admin)     │  (Wearables) │  (Safety Score)│
└──────┬───────┴──────┬───────┴──────┬───────┴────────┬───────┘
       │              │              │                │
       └──────────────┴──────────────┴────────────────┘
                          │
                    ┌─────▼─────┐
                    │  REST API │
                    │ (Express) │
                    └─────┬─────┘
                          │
       ┏━━━━━━━━━━━━━━━━━━┻━━━━━━━━━━━━━━━━━┓
       ▼                  ▼                  ▼
┌──────────────┐  ┌──────────────┐  ┌──────────────┐
│  PostgreSQL  │  │  Blockchain  │  │   AI Model   │
│  (User Data) │  │  (Identity)  │  │ (Prediction) │
└──────────────┘  └──────────────┘  └──────────────┘
```

---

## 🚀 Getting Started

### Prerequisites

- **Node.js** v18+ and npm
- **Flutter** 3.0+ and Dart SDK
- **Python** 3.8+ (for ML services)
- **PostgreSQL** 14+
- **Git**

### Quick Setup

#### 1️⃣ Clone the Repository

```bash
git clone https://github.com/altf4-games/Tour-Raksha.git
cd Tour-Raksha
```

#### 2️⃣ Backend Setup

```bash
cd backend

# Install dependencies
npm install

# Configure environment variables
cp .env.template .env
# Edit .env with your credentials:
# - DATABASE_URL
# - JWT_SECRET
# - GMAIL_USER & GOOGLE_APP_PASSWORD
# - Blockchain network details

# Run Prisma migrations
npx prisma migrate dev
npx prisma generate

# Start the server
npm start
# Development mode: npm run dev
```

**Backend runs on**: `http://localhost:5000`

#### 3️⃣ Frontend (Web Dashboard) Setup

```bash
cd frontend

# Install dependencies
npm install

# Configure environment
cp .env.example .env.local
# Add API URLs and keys

# Start development server
npm run dev
```

**Frontend runs on**: `http://localhost:3000`

#### 4️⃣ Mobile App Setup

```bash
cd app/travel_app

# Install Flutter dependencies
flutter pub get

# Configure API endpoints
# Edit lib/core/config/api_config.dart

# Run on device/emulator
flutter run
```

#### 5️⃣ ML Safety Model Setup

```bash
cd models/safety_score

# Create virtual environment
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate

# Install dependencies
pip install -r requirements.txt

# Train model (optional)
python train.py

# Start API server
python api.py
```

**ML API runs on**: `http://localhost:8000`

#### 6️⃣ Blockchain Smart Contracts (Optional)

```bash
cd contracts/web3-contracts

# Install dependencies
npm install

# Configure network
# Edit hardhat.config.js

# Compile contracts
npx hardhat compile

# Deploy to testnet
npx hardhat run scripts/deploy.js --network goerli
```

---

## 📁 Project Structure

```
Tour-Raksha/
├── app/travel_app/          # Flutter mobile application
│   ├── lib/
│   │   ├── main.dart       # App entry point
│   │   ├── core/           # Core utilities, config
│   │   └── features/       # Feature modules
│   ├── assets/             # Images, fonts
│   └── pubspec.yaml        # Flutter dependencies
│
├── backend/                 # Node.js Express API
│   ├── controllers/        # Route controllers
│   ├── routes/             # API endpoints
│   ├── services/           # Business logic
│   ├── middleware/         # Auth, validation
│   ├── prisma/             # Database schema & migrations
│   └── app.js              # Server entry point
│
├── frontend/                # Next.js admin dashboard
│   ├── src/
│   │   ├── app/            # App router pages
│   │   ├── components/     # React components
│   │   └── lib/            # Utilities
│   └── public/             # Static assets
│
├── contracts/               # Blockchain smart contracts
│   ├── TouristRegistry.sol # Main identity contract
│   └── web3-contracts/     # Hardhat project
│
├── models/safety_score/     # ML safety prediction model
│   ├── train.py            # Model training
│   ├── api.py              # FastAPI service
│   ├── model_utils.py      # ML utilities
│   └── data.csv            # Training dataset
│
└── README.md               # This file
```

---

## 📚 API Documentation

### Authentication

```http
POST /api/users/auth/send-otp
Content-Type: application/json

{
  "email": "tourist@example.com"
}
```

```http
POST /api/users/auth/verify-otp
Content-Type: application/json

{
  "email": "tourist@example.com",
  "otp": "123456"
}
```

### Tourist Management

```http
GET    /api/users              # List all tourists
GET    /api/users/:id          # Get tourist details
POST   /api/users              # Create tourist profile
PUT    /api/users/:id          # Update tourist info
DELETE /api/users/:id          # Delete tourist
```

### KYC & Digital ID

```http
POST /api/users/:id/kyc/aadhar        # Upload Aadhaar
GET  /api/users/:id/kyc/status        # Check KYC status
POST /api/digital-id/generate         # Generate blockchain ID
GET  /api/digital-id/verify/:id       # Verify digital ID
```

### Location & Tracking

```http
POST /api/location/update             # Update tourist location
GET  /api/location/track/:userId      # Get tracking history
POST /api/geofence/check              # Check zone safety
GET  /api/geofence/alerts/:userId     # Get geo-alerts
```

### Safety & Alerts

```http
POST /api/alerts/panic                # Trigger panic alert
GET  /api/alerts/active               # Get active alerts
POST /api/safety/score                # Calculate safety score
GET  /api/safety/zones                # Get risk zones
```

### Trips

```http
POST /api/trips                       # Create trip itinerary
GET  /api/trips/:userId               # Get user trips
PUT  /api/trips/:id                   # Update trip
POST /api/trips/:id/complete          # Mark trip complete
```

### E-FIR (Emergency FIR)

```http
POST /api/efir/generate               # Auto-generate E-FIR
GET  /api/efir/:id                    # Get FIR details
PUT  /api/efir/:id/status             # Update FIR status
```

For complete API documentation, import the Postman collection:

- **File**: `backend/postman/Aadhaar_Verification_API.postman_collection.json`

---

## 🎯 Key Use Cases

### For Tourists

1. **Register** → Verify KYC → Generate Digital ID
2. **Plan Trip** → Set itinerary → Enable tracking
3. **Travel Safely** → Get geo-alerts → Auto safety scoring
4. **Emergency** → Panic button → Instant alert to authorities

### For Authorities

1. **Monitor** → Real-time tourist dashboard
2. **Respond** → Receive panic alerts → Track location
3. **Investigate** → Access digital ID → View trip history
4. **Analyze** → Safety reports → Identify risk zones

### For Families

1. **Opt-in Tracking** → Monitor loved ones
2. **Receive Alerts** → Get notified of zone changes
3. **Emergency Contact** → Listed in tourist profile

---

## 🔬 ML Safety Score Model

The AI model predicts tourist safety scores (0-100) using:

### Features (42+ indicators)

- **Crime Stats**: Murder, kidnapping, robbery, theft rates
- **Natural Disasters**: Floods, earthquakes, cyclones frequency
- **Infrastructure**: Hospitals, police stations per 100k
- **Transportation**: Road accidents, emergency response time
- **Climate**: Rainfall, temperature extremes, weather events
- **Connectivity**: Mobile network, internet, road quality

### Model Performance

- **Algorithm**: Linear Regression
- **Cross-validation R²**: 0.9723 ± 0.0165
- **Test R²**: 0.9728
- **Mean Absolute Error**: 0.7606

### API Usage

```python
import requests

response = requests.post('http://localhost:8000/predict', json={
    "pincode": "110001",
    "murder_rate": 2.3,
    "flood_incidents": 0,
    # ... other features
})

safety_score = response.json()['safety_score']  # 0-100
```

---

## 🌍 Target Users

| User Type                   | Benefits                                                     |
| --------------------------- | ------------------------------------------------------------ |
| **Domestic Tourists**       | Safety monitoring, local language support, emergency SOS     |
| **International Travelers** | KYC integration, real-time tracking, multilingual app        |
| **Solo Travelers**          | Enhanced security, family tracking, 24/7 monitoring          |
| **Elderly/Disabled**        | Voice commands, accessibility features, priority alerts      |
| **Tourism Departments**     | Data analytics, tourist flow management, risk assessment     |
| **Police/Law Enforcement**  | Real-time alerts, digital ID verification, E-FIR automation  |
| **Families**                | Track loved ones, receive safety updates, emergency contacts |

---

## 🛡️ Security & Privacy

- **🔐 End-to-End Encryption**: All data transmissions encrypted
- **🔗 Blockchain Immutability**: Tamper-proof identity records
- **✅ Consent-Based Tracking**: Opt-in location sharing
- **⏰ Time-Limited Data**: Auto-deletion post-trip completion
- **🛡️ GDPR Compliant**: Data protection law adherence
- **🔍 Audit Trails**: Complete activity logging
- **🚫 No Data Selling**: User data never monetized

---

## 🤝 Contributing

We welcome contributions! Please follow these steps:

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit changes (`git commit -m 'Add AmazingFeature'`)
4. Push to branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

### Development Guidelines

- Follow existing code style
- Write tests for new features
- Update documentation
- Ensure all tests pass

---

## 👥 Team Big O(6)

Built with ❤️ by Team Big O(6)

---

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

## 🙏 Acknowledgments

- Tourism departments for problem insights
- Open-source community for amazing tools
- Beta testers for valuable feedback

---

## 📞 Support

For issues, questions, or contributions:

- **Issues**: [GitHub Issues](https://github.com/altf4-games/Tour-Raksha/issues)
- **Discussions**: [GitHub Discussions](https://github.com/altf4-games/Tour-Raksha/discussions)

---

**Made in India 🇮🇳 | Protecting Tourists Worldwide 🌍**
