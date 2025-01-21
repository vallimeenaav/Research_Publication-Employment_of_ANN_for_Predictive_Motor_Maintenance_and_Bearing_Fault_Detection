# Predictive Motor Maintenance Using ANN and Park's Vector Analysis

This repository highlights the research project titled **"Employment of ANN for Predictive Motor Maintenance and Bearing Fault Detection using Park's Vector Analysis."** This work was conducted as part of an undergraduate capstone project in collaboration with Universiti Teknologi PETRONAS and Vellore Institute of Technology and has been published in IEEE Xplore.

> 📄 **Published Paper**: [Employment of ANN for Predictive Motor Maintenance and Bearing Fault Detection using Park's Vector Analysis](https://ieeexplore.ieee.org/document/9915683)

---

## Overview
This project leverages **Motor Current Signature Analysis (MCSA)** combined with **Park's Vector Analysis** and **Artificial Neural Networks (ANN)** to classify the health of three-phase industrial motors. It addresses the challenges of real-time, non-invasive motor fault detection using lightweight and computationally efficient solutions that can be deployed on edge devices.

### Key Contributions:
- **Non-invasive predictive maintenance**: Utilizes motor current signals instead of invasive sensors.
- **Lightweight ANN classifier**: Optimized to run on low-cost hardware like Raspberry Pi.
- **Industrial impact**: Real-time motor health monitoring in remote or resource-constrained environments.

---

## Repository Content
This repository includes:
1. **Final_Report.pdf**: Comprehensive documentation of the methodology, hardware design, and results.
2. **Presentation.pptx**: A summary presentation of the project and its key findings.
3. **Published_Paper_Link**: The [published research paper](https://ieeexplore.ieee.org/document/9915683) on IEEE Xplore.
4. **Screenshots and Visuals**:
   - Example Park Vector plots showcasing healthy and unhealthy motor states.
   - Hardware setup diagrams.
5. **Hardware Design**:
   - Circuit diagrams and design choices for Raspberry Pi integration.

> **Note**: Due to restrictions, the dataset and code files are not publicly shared.

---

## Problem Statement
Industrial motors, particularly induction motors, experience significant wear and tear over time. Bearing faults constitute over 40% of motor failures and can lead to costly downtime. Existing methods for fault detection are either invasive, expensive, or lack accuracy.

### Objectives:
1. Design a non-invasive system for bearing fault detection using motor current signals.
2. Implement a lightweight ANN model for fault classification.
3. Deploy the model on edge devices like Raspberry Pi for real-time use.

---

## Technical Highlights

### Hardware Setup
- **Industrial Motor Components**:
  - Three-phase induction motor.
  - Clamp Transducers (LEM RT-2000), Rogowski Coils.
  - Signal Integrator (LEM AI-PMUL) for voltage mapping.
- **Edge Device**: Raspberry Pi 4 Model B with 8GB RAM.
- **Power Supply**: Regulated dual-voltage source (5V and 24V) to power Raspberry Pi and signal integrator.

### Software Specifications
- **Programming Language**: Python
- **Libraries and Frameworks**: TensorFlow, Keras, Matplotlib
- **Operating System**: 64-bit Raspbian OS (Debian-based).

---

## Methodology
1. **Data Collection**:
   - Motor current data collected from industrial setups.
   - Converted into Park Vector plots representing healthy and faulty motor states.
2. **Model Development**:
   - ANN model with a 3-layer architecture:
     - **Input Layer**: Park Vector plots.
     - **Hidden Layers**: ReLU activation functions.
     - **Output Layer**: Sigmoid activation function for binary classification.
   - Training Accuracy: >99%.
3. **Deployment**:
   - ANN model optimized for low computational complexity.
   - Successfully deployed on Raspberry Pi for real-time fault classification.

---

## Results
### Performance Metrics
- **Accuracy**: >99.99% on the test dataset.
- **Confusion Matrix**:
  
| Healthy   | Unhealthy |
|-----------|-----------|
| 16        | 0         |
| 0         | 20        |

- 100% precision, recall, and F1 score.

### Deployment Impact
- **Training Time**:
- **Raspberry Pi**: 1.3 minutes.
- **Desktop**: 50 seconds.
- **Cloud (Google Colab)**: 36 seconds.
- **Real-world Integration**:
- Low-cost deployment.
- Suitable for remote industrial sites with limited resources.

---

## Applications
This project demonstrates significant potential in:
- **Industrial Automation**: Ensures uninterrupted operations by predicting faults before they occur.
- **Cost Efficiency**: Reduces the need for full-scale shutdowns and maintenance cycles.
- **Edge Computing**: Demonstrates the feasibility of deploying AI models on low-resource devices.

---

## How to Use
Although the dataset and code are classified, the following resources are available:
1. **Final_Report.pdf**: Detailed explanation of the methodology and implementation.
2. **Park Vector Plots**: Example visuals to understand the input-output relationship.
3. **Hardware Guide**: Step-by-step setup for deploying ANN models on Raspberry Pi.

For further inquiries, feel free to reach out through the repository's contact section.

---

## Acknowledgments
This project was made possible through the collaborative efforts of:
- **Vellore Institute of Technology, India**
- **Universiti Teknologi PETRONAS, Malaysia**

Special thanks to our advisors:
- Dr. Sujatha R.
- Dr. Madiah Omar.

---

## License
This project is licensed under the **MIT License**.


