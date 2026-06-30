DrowsyGuard Pro - Complete Technical Architecture
1. Artificial Intelligence (AI) Model
The application integrates Artificial Intelligence through Google's MediaPipe Face Mesh. A pre-trained deep learning model detects 468 facial landmarks from each webcam frame. The project performs AI inference only; it does not train a new model.
2. Machine Learning Model
Machine Learning is used through the embedded MediaPipe Face Mesh model. The model was previously trained by Google using large face datasets. The application performs only prediction (inference). No custom dataset or training process is included.
3. Deep Learning
The MediaPipe Face Mesh model is based on deep neural networks for facial landmark estimation. CNN-based feature extraction is used internally by MediaPipe to accurately predict landmark positions.
4. Computer Vision
Computer Vision processes live webcam images. Face landmarks are extracted and used to calculate Eye Aspect Ratio (EAR), Mouth Aspect Ratio (MAR), head tilt, lighting level, and fatigue indicators.
5. Detection Algorithms
• EAR for eye closure
• MAR for yawning
• Head tilt estimation
• Head pose calibration
• Ambient light estimation
• Fatigue score computation
• Rule-based decision engine.
6. Protocols and APIs
HTTP/HTTPS (library download), WebRTC getUserMedia (camera), HTML5 Canvas API, Web Audio API, Web Speech API (optional voice), JavaScript DOM API, jsPDF library. Processing is local after libraries are loaded.
7. Complete AI Pipeline
Camera → Webcam Frames → Brightness Analysis → Optional Night Mode Enhancement → MediaPipe Face Mesh → 468 Facial Landmarks → Feature Extraction (EAR, MAR, Head Tilt) → Rule-Based Fatigue Engine → Fatigue Score → Alerts (Visual, Audio) → Session Statistics → PDF Trip Report.
8. Layered Architecture
Presentation Layer: HTML/CSS UI
Application Layer: JavaScript
Computer Vision Layer: MediaPipe Face Mesh
Feature Extraction Layer: EAR, MAR, Head Tilt
Decision Layer: Threshold-based fatigue detection
Alert Layer: Visual overlays, alarms
Reporting Layer: PDF report generation
Hardware Layer: Camera, Display, Speaker.
9. Full System Architecture
Driver → Webcam → Browser → Frame Capture → Brightness Detection → Night Mode Enhancement → MediaPipe AI Model → Landmark Detection → EAR/MAR/Head Tilt Calculation → Fatigue Decision Engine → Alert Manager → Dashboard → PDF Report.
10. AI vs ML vs CV
AI: Yes
Machine Learning: Yes (pre-trained model)
Deep Learning: Yes
Computer Vision: Yes
Custom Model Training: No
Cloud AI: No
Edge AI: Yes (browser-side inference).
11. Technologies
HTML5, CSS3, JavaScript, MediaPipe Face Mesh, Canvas API, WebRTC, jsPDF, Web Audio API.
