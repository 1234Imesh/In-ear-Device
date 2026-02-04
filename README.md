# 🧠 In-Ear EEG / ECG Signal Processing Framework

This repository presents a **signal-processing and analysis framework** developed for a **wearable in-ear EEG/ECG device**, designed for **real-world, motion-rich environments** rather than controlled laboratory settings.

Unlike conventional scalp EEG systems, in-ear recordings are inherently affected by **head motion, jaw activity, facial EMG, and sensor displacement**. To explicitly model and mitigate these effects, the system integrates **Inertial Measurement Unit (IMU) data** alongside electrophysiological signals.

---

## 🔬 Project Focus

The project investigates how **motion and physiological artifacts couple into in-ear EEG/ECG signals**, and how these dependencies can be **quantified, interpreted, and reduced** using principled signal-processing methods.

Key goals include:
- Preserving **true neural and cardiac activity**
- Identifying **motion-induced contamination**
- Enabling **long-term, comfortable, wearable monitoring**

---

## ⚙️ Core Methodology

- High-rate EEG acquisition (up to **10 kHz**) with physiologically informed filtering  
- Optional **60 Hz notch filtering** for environmental interference  
- **IMU–EEG temporal synchronization** using normalized time alignment  
- Signal quality assessment via **variance-based SNR**  
- Motion–signal dependency analysis using:
  - Pearson correlation (linear coupling)
  - Canonical Correlation Analysis (multivariate coupling)
  - Mutual Information (non-linear coupling)
- Dependency reduction using:
  - **Adaptive filtering** (real-time oriented)
  - **Independent Component Analysis (ICA)** for offline separation

---

## 🧪 Design Philosophy

- **Physics-driven signal processing**, not black-box ML  
- Motion treated as a **measurable input**, not a nuisance to ignore  
- Emphasis on **interpretability, stability, and deployability**  
- Algorithms selected with **wearable constraints** in mind (latency, power, robustness)

---

## 🎯 Intended Use Cases

- Long-term EEG monitoring during wakefulness and sleep  
- Motion-aware wearable neurotechnology  
- Brain–body interaction and artifact modeling studies  
- Foundations for **real-time ANC and closed-loop neurophysiological systems**

---

## 🚧 Project Status

Active research prototype.  
Ongoing work includes improved adaptive filtering under gravitational effects, multi-recording validation, and real-time embedded deployment.

---

## 📜 License

Intended for **research and educational use**.
