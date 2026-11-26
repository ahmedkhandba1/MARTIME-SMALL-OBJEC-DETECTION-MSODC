# PhyMSOD: Physics-Aware Maritime Small Object Detection using Camera-RADAR Fusion

## Introduction

PhyMSOD (Physics Maritime Radar–Vision Fusion) is a physics-guided adaptive multi-sensor fusion framework designed for robust maritime object detection, tracking, and classification in challenging coastal and port environments.

The framework combines camera features and radar features using adaptive weighting based on environmental conditions and radar physics parameters.


---

#  Adaptive Radar–Camera Feature Fusion Architecture

<img width="1600" height="900" alt="MAIN_PROCESS" src="https://github.com/user-attachments/assets/12ccc518-cb1c-4cb4-95dc-51a00363fff9" />


Where:

- **F_camera** → Extracted camera features  
- **F_radar** → Extracted radar features  
- **SA(F_radar)** → Shuffle Attention refined radar features  
- **α_c(P_e)** → Adaptive camera confidence weight from environmental parameters  
- **α_r(P_r)** → Adaptive radar confidence weight from radar physics parameters  

The framework improves maritime perception under:
- Fog and low visibility
- Sea clutter and glare
- Long-range small object detection
- Day/Night environmental changes
- Dynamic maritime environments


## Description

This figure presents the complete MRVFusion architecture.

### Key Components
- Camera input processed using CNN backbone
- Radar input processed using radar encoder
- Environmental adaptive weighting for camera reliability
- Radar physics adaptive weighting for radar reliability
- Shuffle Attention (SA) module for radar feature refinement
- Physics-guided feature fusion
- Final maritime object detection and classification

### Environmental Variables \(P_e\)
- Fog / Visibility
- Rain
- Day/Night illumination
- Glare
- Wave and sea-state conditions

### Radar Physics Variables \(P_r\)
- Range
- Doppler velocity
- Bearing angle
- Signal-to-noise ratio (SNR)
- Sea clutter

This framework enables adaptive sensor confidence balancing depending on maritime conditions.

---

# Maritime Sensing Workflow
<img width="1536" height="1024" alt="ChatGPT Image Jun 3, 2026, 10_33_36 PM" src="https://github.com/user-attachments/assets/df5cc3fb-e08f-4928-a019-85a4780891a7" />


## Description

This image demonstrates the complete maritime sensing workflow.

### Included Outputs
1. Original maritime camera image
2. Marine radar representation
3. REVMap radar intensity visualization
4. Final object detection and classification output

### Detected Maritime Objects
- Breakwaters
- Small boats
- Leisure boats
- Cargo ships
- Navigation buoys
- Channel buoys
- Jet skis / PWC

The REVMap visualization helps represent radar intensity distributions and improves target interpretation.

---

# Long-Range Maritime Small Object Detection
<img width="1693" height="929" alt="plane_multiple_output" src="https://github.com/user-attachments/assets/5c1064aa-6475-45cb-85c4-16652b13b4e8" />

## Description

This figure demonstrates long-range maritime object analysis using the proposed framework.

### Detected Objects
- Small fishing boats
- Speed boats
- Distant small vessels
- Cargo ships / tankers
- Offshore platforms
- Marker buoys
- Tiny bright targets near horizon

### Deep Analysis
- Small object detection at long range
- Horizon-based target analysis
- Maritime clutter handling
- Tiny target localization
- Reduced false alarms

This demonstrates the capability of MRVFusion for detecting very small maritime targets under hazy and cluttered environments.


The framework is optimized for real-time maritime surveillance and autonomous unmanned surface vehicle (USV) navigation systems.

---

## Video Clip

The clip shows radar-guided zoom and object classification
[Watch the demonstration video]


https://github.com/user-attachments/assets/7f008683-b550-4298-b2b5-bc87348ba134





---

# Applications

- Autonomous Unmanned Surface Vehicles (USVs)
- Maritime surveillance systems
- Coastal monitoring
- Port navigation safety
- Collision avoidance systems
- Radar-camera sensor fusion research
- Small object maritime detection

---

# Research Focus

The research focuses on:
- Physics-guided sensor fusion
- Maritime AI perception
- Multi-modal deep learning
- Radar-camera fusion
- Tiny maritime object detection
- Adaptive environmental awareness
- Real-time maritime navigation systems


---

## Source Code

The manuscript is currently under review. This repository will be updated with the source code once the paper is published.

---

## Author Affiliation

PhD Research Scholar  
BITS Pilani Dubai Campus
