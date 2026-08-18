
# SMART FACTORY GUARDIAN

### Autonomous Predictive Maintenance & Digital Twin System

SMART FACTORY GUARDIAN is a Python-based **Industry 4.0 predictive maintenance system** that simulates a virtual manufacturing machine, monitors multiple sensor parameters, detects abnormal behaviour, calculates machine health, diagnoses potential faults, and generates automated maintenance recommendations.

The project demonstrates how **NumPy, Pandas, SciPy, and Matplotlib** can work together to create an automated industrial monitoring solution.

---

## 🚀 Features

* ⚙️ Automatic industrial sensor data simulation
* 🌡️ Temperature monitoring
* 📳 Vibration monitoring
* 🔄 RPM monitoring
* ⚡ Power consumption monitoring
* 📊 Pandas-based data processing
* 🧪 SciPy-based statistical anomaly detection
* 🩺 Automated Machine Health Score
* 🚨 Automatic anomaly identification
* 🔍 Rule-based fault diagnosis
* 📈 Machine health trend visualization
* 🛠️ Automated maintenance recommendations
* 🏭 Simplified Digital Twin concept
* 📉 Professional Matplotlib diagnostic dashboard

---

## 🧠 System Architecture

```text
             VIRTUAL MANUFACTURING MACHINE
                         │
                         ▼
              AUTOMATIC SENSOR SIMULATION
                         │
          ┌──────────────┼──────────────┐
          ▼              ▼              ▼
     Temperature      Vibration        RPM
                         │
                         ▼
                  Power Consumption
                         │
                         ▼
                  Pandas DataFrame
                         │
                         ▼
                Data Preprocessing
                         │
                         ▼
              SciPy Anomaly Detection
                         │
                         ▼
               Machine Health Score
                         │
                         ▼
                Fault Diagnosis
                         │
              ┌──────────┴──────────┐
              ▼                     ▼
        Maintenance Action      Visualization
```

---

## 🛠️ Technologies Used

| Technology       | Purpose                                     |
| ---------------- | ------------------------------------------- |
| **Python**       | Core programming language                   |
| **NumPy**        | Numerical operations and sensor simulation  |
| **Pandas**       | Data organization and analysis              |
| **SciPy**        | Statistical analysis and anomaly detection  |
| **Matplotlib**   | Data visualization and diagnostic dashboard |
| **Google Colab** | Development and execution environment       |

---

## ⚙️ How It Works

### 1. Sensor Simulation

The system automatically generates synthetic industrial sensor data representing a virtual manufacturing machine.

The monitored parameters are:

* Temperature — °C
* Vibration — mm/s
* RPM — revolutions per minute
* Power — kW

The machine initially operates under normal conditions. A gradual degradation scenario is then introduced to simulate a developing machine fault.

### 2. Data Processing

The generated sensor readings are stored in a **Pandas DataFrame**.

Rolling averages and statistical information are calculated to identify underlying trends while reducing the effect of random sensor noise.

### 3. Anomaly Detection

**SciPy's statistical functions** are used to calculate Z-scores.

A significantly high absolute Z-score indicates that a sensor reading differs considerably from normal behaviour.

This allows the system to automatically identify abnormal operating conditions.

### 4. Machine Health Score

A composite health score from **0–100%** is calculated using the condition of multiple sensors.

The weighted model is:

```text
Temperature → 30%
Vibration   → 30%
RPM         → 20%
Power       → 20%
```

The machine is classified as:

```text
75–100%  → NORMAL
50–74%   → WARNING
0–49%    → CRITICAL
```

### 5. Fault Diagnosis

The system analyzes sensor conditions and their relationships to identify possible machine problems such as:

* Overheating
* Bearing failure
* Mechanical vibration
* RPM degradation
* Excessive load
* General machine degradation

### 6. Maintenance Recommendation

Based on the machine's current condition, the system automatically generates an appropriate recommendation, ranging from continued monitoring to immediate inspection.

---

## 📊 Visualization

Matplotlib generates a diagnostic dashboard showing:

* Temperature trend
* Vibration trend
* RPM trend
* Power consumption
* Machine Health Score
* Critical operating thresholds
* Degradation period

These visualizations allow the machine's condition to be understood quickly.

---

## 🏭 Industry 4.0 Relevance

This project demonstrates several important Industry 4.0 concepts:

### Predictive Maintenance

Instead of waiting for a machine to fail, sensor data is continuously analyzed to identify early signs of degradation.

### Digital Twin

The virtual machine acts as a simplified **Digital Twin**, representing the behaviour of a physical manufacturing asset through simulated sensor data.

### Smart Automation

The system automatically performs:

```text
Data Generation
      ↓
Data Processing
      ↓
Anomaly Detection
      ↓
Health Assessment
      ↓
Fault Diagnosis
      ↓
Maintenance Recommendation
```

No manual sensor dataset is required.

### Data-Driven Decision Making

Maintenance decisions are generated from numerical sensor analysis rather than manual observation.

---

## 📁 Project Structure

```text
SMART-FACTORY-GUARDIAN/
│
├── SMART_FACTORY_GUARDIAN.ipynb
├── README.md
└── requirements.txt
```

---

## ▶️ Running the Project

The project can be executed directly in **Google Colab**.

### Requirements

```text
Python 3.x
NumPy
Pandas
SciPy
Matplotlib
```

Install dependencies if required:

```bash
pip install numpy pandas scipy matplotlib
```

Then open:

```text
SMART_FACTORY_GUARDIAN.ipynb
```

and run the notebook cells sequentially.

---

## 📌 Example Output

```text
============================================================
        SMART FACTORY GUARDIAN
        MACHINE DIAGNOSTIC REPORT
============================================================

Machine ID        : MFG-001
Operating Cycles  : 300

Latest Sensor Readings
------------------------------------------------------------
Temperature       : 84.60 °C
Vibration         : 6.70 mm/s
RPM               : 1378
Power             : 7.10 kW

Machine Health
------------------------------------------------------------
Health Score      : 47.80 %
Machine Status    : CRITICAL
Anomalies Found   : 38

Automatic Diagnosis
------------------------------------------------------------
Likely Fault      : Bearing Failure
Confidence        : 87 %

Maintenance Action
------------------------------------------------------------
Inspect bearing and rotating components immediately.
============================================================
```

*Example values are illustrative; actual results depend on the simulation.*

---

## 🎯 Objectives

The project aims to demonstrate:

1. Application of Python in smart manufacturing
2. Numerical computation using NumPy
3. Industrial data analysis using Pandas
4. Statistical anomaly detection using SciPy
5. Engineering visualization using Matplotlib
6. Predictive maintenance concepts
7. Digital Twin fundamentals
8. Automated industrial decision-making

---

## 🔮 Future Scope

The current system uses simulated sensor data. It can be extended into a real-world predictive maintenance platform by integrating:

* IoT sensors
* ESP32/Arduino
* Real-time machine data
* MQTT communication
* Database storage
* Machine Learning models
* Deep Learning-based fault prediction
* Real-time dashboards
* Cloud monitoring
* Remaining Useful Life (RUL) prediction

---

## 👩‍💻 Author

**Shreeya Routray**
B.Tech — Mechanical & Smart Manufacturing Engineering
Veer Surendra Sai University of Technology (VSSUT), Burla

---

### ⭐ Project Concept

> **“From sensor data to intelligent maintenance decisions — automatically.”**
