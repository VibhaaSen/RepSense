# RepSense
Thigh-mounted wearable for real-time squat rep detection using IMU sensor fusion.
# 🦵 RepSense — Smart Squat Accountability Wearable

RepSense is a thigh-mounted wearable system that uses real-time motion sensing to detect and count full squat repetitions with high accuracy. Unlike traditional fitness trackers that estimate activity through generalized movement, RepSense focuses specifically on lower-body biomechanics to recognize complete squat motion patterns.

Using a 6-axis IMU (accelerometer + gyroscope) and sensor-fusion algorithms, the system continuously tracks thigh angle, rotational movement, and squat depth throughout each repetition. The firmware analyzes this data in real time to determine when a user:
- begins descent
- reaches valid squat depth
- returns to standing position
- completes a full repetition

The goal of RepSense is to bring accountability and precision to strength training by ensuring that every recorded rep represents a true, full range-of-motion squat.

---

## 🚀 Features

- Real-time squat rep detection
- IMU-based motion tracking
- Sensor fusion using accelerometer + gyroscope data
- Full-range squat validation
- Lightweight wearable form factor
- Low-cost embedded hardware implementation
- Expandable exercise recognition platform

---

## ⚙️ System Overview

### Hardware
- 6-axis IMU sensor (accelerometer + gyroscope)
- Microcontroller for real-time processing
- Battery-powered wearable system
- Optional vibration feedback module
- Optional display/debug interface

### Software
- Sensor fusion using complementary filtering
- Angle estimation from accelerometer + gyroscope data
- State-machine-based rep detection
- Threshold-based squat validation logic
- Noise filtering and motion smoothing

---

## 🧠 How It Works

RepSense continuously monitors femur orientation during exercise.

The system detects:
1. Upright standing position
2. Downward rotational movement
3. Squat depth threshold
4. Upward return to standing position

Once a complete movement cycle is confirmed, the firmware registers a valid squat repetition.

This allows the device to distinguish between:
- partial reps
- full reps
- random leg movement
- actual squat motion patterns

---

## 📊 Why This Matters

Most wearable fitness trackers are optimized for:
- steps
- cardio
- generalized activity tracking

RepSense focuses on an underserved problem in fitness technology:

> Accurate strength-training movement validation.

The project aims to provide:
- workout accountability
- consistent rep tracking
- improved training feedback
- potential rehabilitation and athletic applications

---

## 🔮 Future Development

Potential future features include:
- Lunge detection
- Split squat tracking
- Tempo analysis
- Rep quality scoring
- Mobile app integration
- Machine-learning-based movement classification
- Rehab and physical therapy support

---

## 📁 Planned Repository Structure

```text
RepSense/
│
├── README.md
├── firmware/
├── hardware/
├── docs/
├── images/
├── data/
└── tests/
