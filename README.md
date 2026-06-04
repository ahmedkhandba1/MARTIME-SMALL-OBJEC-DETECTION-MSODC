# MRVFusion: Physics-Guided Maritime Radar–Vision Fusion Framework

## Introduction

MRVFusion (Maritime Radar–Vision Fusion) is a physics-guided adaptive multi-sensor fusion framework designed for robust maritime object detection, tracking, and classification in challenging coastal and port environments.

The framework combines camera features and radar features using adaptive weighting based on environmental conditions and radar physics parameters.


---

# 1. Adaptive Radar–Camera Feature Fusion Architecture

![MRVFusion Architecture]
The proposed fusion equation is:

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

# 2. Maritime Radar and REVMap Generation

![Radar and REVMap]


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

# 3. Long-Range Maritime Small Object Detection

![Long Range Maritime Detection](ChatGPT%20Image%20Jun%203,%202026,%2010_33_36%20PM.png)

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

---

# 4. Plane Radar Image and REVMap Visualization

![Plane Radar and REVMap](plane_radar_multiple.png)

## Description

This image shows simulated plane radar and REVMap outputs.

### Features
- Radar PPI-style visualization
- Circular range rings
- Target intensity mapping
- REVMap heat visualization
- Radar point target representation

The REVMap representation improves visibility of weak radar targets and assists in radar feature learning.

---

# 5. Maritime Object Detection and Classification

![Object Detection and Classification](plane_multiple_output.png)

## Description

This figure presents detailed maritime object detection and classification results.

### Classification Categories
- Small fishing boats
- Leisure boats
- Speed boats
- Cargo ships / tankers
- Offshore platforms
- Navigation buoys
- Tiny distant targets
- Sea clutter regions

### Detection Capabilities
- Multi-object detection
- Long-range target analysis
- Tiny object recognition
- Maritime scene understanding
- Clutter-aware classification

The framework is optimized for real-time maritime surveillance and autonomous unmanned surface vehicle (USV) navigation systems.

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

# Future Work

Future extensions of MRVFusion may include:
- Physics-informed neural networks (PINNs)
- AIS integration
- COLREG-compliant autonomous navigation
- Real-time tracking and trajectory prediction
- Multi-frame radar temporal fusion
- Thermal and infrared sensor integration

---

# Author

Ahmed Khan  
PhD Research Scholar  
BITS Pilani Dubai Campus

