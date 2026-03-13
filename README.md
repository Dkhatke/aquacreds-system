# AquaCreds – Blue Carbon MRV System

AquaCreds is an AI and blockchain-based platform for monitoring, reporting, and verifying (MRV) blue carbon ecosystems such as mangroves.

Smart India Hackathon 2025 Finalist.

## System Components

### 1. AI Model
Satellite imagery analysis for mangrove biomass estimation.

Repository:
[https://github.com/Dkhatke/aquacreds-ml](https://github.com/Dkhatke/aquacreds-ml)

### 2. Blockchain Registry
Smart contracts store verified carbon credits on the Polygon blockchain.

Repository:
[https://github.com/Dkhatke/aquacreds-blockchain](https://github.com/Dkhatke/aquacreds-blockchain)

### 3. Frontend Dashboard
Web interface for monitoring carbon credit issuance and ecosystem metrics.

Repository:
[https://github.com/Dkhatke/final_aquacreds_frontend](https://github.com/Dkhatke/final_aquacreds_frontend)

## System Architecture

Satellite Data → AI Model → Biomass Estimation → Smart Contract → Carbon Credit Registry → Dashboard


# AquaCreds — Blockchain-Based Blue Carbon Registry & MRV System

AquaCreds is a **blockchain-powered Monitoring, Reporting, and Verification (MRV) platform** designed to bring transparency, trust, and scalability to **blue carbon ecosystems** such as **mangroves, seagrass, and salt marshes**.

The platform integrates **AI/ML, satellite imagery, blockchain, and decentralized storage** to verify carbon sequestration projects and issue **tokenized carbon credits**.

This project was developed for **Smart India Hackathon 2025 – Problem Statement SIH25038**. 

---

# Problem Statement

Blue carbon ecosystems store carbon **up to 10× faster than terrestrial forests**, but current carbon credit verification systems suffer from:

* Lack of transparency
* Slow manual verification
* Risk of greenwashing
* High verification costs

AquaCreds solves this using **AI-based verification + blockchain immutability**.

---

# Key Features

## 1. AI-Based MRV (Monitoring, Reporting & Verification)

* Upload **geotagged plantation photos**
* Extract EXIF metadata:

  * GPS Coordinates
  * Timestamp
  * Device ID
* AI models analyze ecosystem health

Parameters calculated:

* NDVI (Vegetation Index)
* NDWI (Water Index)
* Canopy Cover
* Ecosystem classification

AI models used:

* CNN
* U-Net segmentation

---

## 2. Satellite Validation

The system validates ground photos using **satellite imagery**:

Satellites used:

* Sentinel-1
* Sentinel-2
* Landsat 8/9

Satellite and field data are compared to prevent **fraudulent submissions**.

---

## 3. Blockchain-Based Carbon Registry

All verified MRV records are stored on **Polygon Blockchain**.

Blockchain ensures:

* Immutable records
* Transparent verification
* Tamper-proof carbon credit issuance

Smart contracts handle:

* Carbon credit token minting
* Verification approval
* Marketplace transactions

Token Standards:

* **ERC-20** → Carbon Credit Tokens
* **ERC-721** → Plantation NFT Records

---

## 4. Decentralized Storage

Images and datasets are stored using **IPFS**.

Process:

```
Image Upload → IPFS Storage → Hash generated → Hash stored on Polygon
```

Benefits:

* Decentralized storage
* Tamper-proof data
* Reduced blockchain storage cost

---

## 5. Carbon Credit Marketplace

A built-in **tokenized marketplace** allows:

* Corporates to purchase carbon credits
* NGOs to sell verified carbon offsets
* Governments to monitor credit issuance

Marketplace features:

* Reverse Auction system
* Tokenized carbon credits
* Transparent transactions

---

# System Architecture

```
User (NGOs / Communities)
        │
        ▼
Field Data Upload (Photos + Metadata)
        │
        ▼
EXIF Verification
        │
        ▼
AI/ML Analysis
(NDVI, NDWI, Canopy, Ecosystem Detection)
        │
        ▼
Satellite Image Validation
        │
        ▼
Carbon Estimation (AGB + BGB)
        │
        ▼
MRV Report Generation
        │
        ▼
Hash stored on Polygon Blockchain
        │
        ▼
Carbon Credit Issuance
        │
        ▼
Marketplace Trading
```

---

# Tech Stack

## Frontend

* React.js
* React Native
* Chart.js

---

## Backend

* Node.js
* Express.js
* GraphQL
* MongoDB

---

## Blockchain

* Solidity
* Hardhat
* Polygon
* MetaMask
* OpenZeppelin

---

## AI / ML

* Python
* TensorFlow
* PyTorch
* Google Earth Engine
* Remote sensing models

---

## Storage

* IPFS

---

## APIs

* Satellite APIs
* Drone APIs
* Web3Auth

---

# Carbon Estimation Model

Carbon estimation is calculated using **IPCC and MoEFCC formulas**.

Steps:

1. Estimate **Canopy Density**
2. Convert to **Above Ground Biomass (AGB)**
3. Calculate **Below Ground Biomass (BGB)**
4. Convert biomass to **CO₂ equivalent (tCO2e)**

These values determine **carbon credits issued**.

---

# Security & Transparency

The system prevents fraud using:

* EXIF metadata validation
* AI image classification
* Satellite verification
* Blockchain immutability
* IPFS decentralized storage

This reduces **greenwashing in carbon markets**.

---

# Impact

## Environmental

* Blue carbon ecosystem restoration
* Carbon sequestration
* Coastal protection

## Economic

* Carbon credit revenue
* Sustainable income for coastal communities
* Investment in climate solutions

## Social

* Job creation
* Community empowerment
* Local ecosystem conservation

---

# Target Users

* NGOs working on mangrove restoration
* Coastal communities
* Corporates aiming for **net-zero goals**
* Government agencies
* Climate researchers

---


# Unique Innovations

AquaCreds introduces several novel ideas:

* AI Fraud Detection (Photo + Satellite)
* Reverse Auction Carbon Financing
* Blockchain MRV Registry
* Tokenized Carbon Marketplace
* Decentralized Storage via IPFS

---

# Future Scope

* Drone-based monitoring
* Global blue carbon registry
* DAO governance for carbon projects
* Integration with international carbon markets

---

# Team VISSDOM

Developed for **Smart India Hackathon 2025**

Team ID: **82991**

Project Theme: **Clean and Green Technology**

