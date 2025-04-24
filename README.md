# Hypoxia-Induced Speech Slurring Classification

A deep learning approach to classify hypoxia-induced slurring in pilot's speech using  Convolutional Neural Networks.

<img src="images/a350_cockpit.jpg" alt="a350 flightdeck" style="max-width: 500px;"/>

### Cabin Pressure and Aviation Safety
Commercial aircraft cabins are pressurized to allow passengers to breathe comfortably at high altitudes. These aircraft have sophisticated systems to monitor cabin pressure and oxygen levels, with automated safety features like oxygen mask deployment during depressurization events.

However, in smaller aircraft and particularly military aircraft, the warning systems are not as sophisticated. Pilots are responsible for monitoring cabin pressure and oxygen levels themselves. While pilots are trained to recognize hypoxia symptoms, they are not always immediately obvious to those experiencing them.

### The Problem of Hypoxia
Hypoxia occurs when the body doesn't get enough oxygen. One common symptom of hypoxia is the slurring of speech (medically known as dysarthria). During hypoxia incidents, air traffic controllers often notice the pilot's speech becoming progressively more slurred before they realize there might be a problem.

## Project Overview
This project implements a Convolutional Neural Network to classify speech as either dysarthric or non-dysarthric. The system could potentially be used by air traffic controllers to detect hypoxia before it becomes severe, providing an additional layer of safety monitoring.

### Technical Implementation
- Uses the TORGO Dataset for training
- Implements feature extraction including:
  - MFCC features with deltas
  - Spectral features (centroid, bandwidth, rolloff)
  - Chroma features
  - Zero crossing rate
- Employs a CNN architecture for classification
- Achieves 95% accuracy with balanced precision and recall across both classes

## Results
- Accuracy: 95%
- Precision: 0.95 (both classes)
- Recall: 0.95 (both classes)
- F1-Score: 0.95
- AUC: 0.9941