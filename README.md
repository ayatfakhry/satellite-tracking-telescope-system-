# 🚀 Autonomous Satellite Tracking System

## 📌 Overview
This project presents a complete software-based autonomous satellite tracking system using orbital mechanics, STK simulation, and real-time TLE data.

The system predicts satellite motion, evaluates visibility conditions, and automatically selects the best satellite pass for tracking using both traditional scoring and AI-based optimization.

---

## 🧠 Key Features

- 🛰️ STK-based orbit simulation (5 different orbits)
- 📡 Orbit propagation using RK4 method
- 📊 Error analysis (RMSE, Mean Error)
- 🌍 Ground track visualization
- 📍 AER calculation (Azimuth, Elevation, Range)
- 🎯 Autonomous best-pass selection
- 🤖 AI-based orbit selection (Random Forest)
- 📡 Real-time tracking using TLE data
- 🧭 Telescope pointing angle generation
- 📈 Decision comparison (Traditional vs AI)

---

## ⚙️ Methodology

### 1. Orbit Generation
Satellite orbits are generated using STK and exported as position/velocity data.

### 2. Orbit Prediction
The system uses RK4 numerical integration to predict satellite motion.

### 3. Tracking Analysis
- Ground station defined (Beni Suef, Egypt)
- AER values computed
- Visibility windows determined (AOS / LOS)

### 4. Decision System
Two approaches are used:
- Traditional tracking score
- AI-based model (Random Forest)

### 5. Final Decision
The system selects the best orbit for tracking automatically.

---

## 📊 Results

- Accurate orbit prediction with low RMSE
- Successful identification of optimal tracking orbit
- AI model confirms and enhances decision-making
- Real-time satellite tracking using TLE data

---

## 🤖 AI Optimization

A Random Forest regression model was used to improve the tracking decision.  
The model evaluates:

- Maximum elevation
- Visibility duration
- Minimum range

---

## 🔮 Future Work

- Integration with hardware (motors + Arduino/ESP32)
- Real-time tracking with live satellite feeds
- AI model improvement with larger datasets
- Fully autonomous telescope system

---

## 🛠️ Technologies Used

- Python
- STK (Systems Tool Kit)
- NumPy, Pandas, Matplotlib
- Scikit-learn (AI Model)
- Skyfield (TLE Tracking)

---

## 📁 Project Structure
