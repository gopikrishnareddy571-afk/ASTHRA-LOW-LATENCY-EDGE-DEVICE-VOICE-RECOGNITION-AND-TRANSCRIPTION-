# ASTHRA

#Low-Latency Voice Activator for Edge Devices

**SIH Problem Statement: SIH26172  
**Team: TOP GUN  
**Team Number: 160920



🚀 Overview

ASTHRA is a low-latency, voice-activated edge device designed for efficient keyword detection on resource-constrained embedded systems.

The device continuously listens for the keyword **"ASTHRA"** using an INMP441 I2S MEMS microphone. Once detected, it activates speech capture and forwards the recorded speech to an ASR system for transcription.

The wake-word detection runs locally on the ESP32, reducing unnecessary communication and enabling fast activation.

---

## 🎯 Key Features

- Low-latency wake-word detection
- Keyword: **ASTHRA**
- ESP32-based edge processing
- INMP441 I2S MEMS microphone
- Lightweight CNN model
- MFCC-based audio feature extraction
- INT8 TensorFlow Lite model
- OLED status display
- Wi-Fi communication with ASR server
- Dedicated MEMS microphone dataset
- Designed for low-resource edge deployment

---

## 🧠 Working Principle

```text
INMP441 Microphone
        ↓
   Audio Capture
        ↓
   MFCC Extraction
        ↓
  CNN Wake-Word Model
        ↓
   ASTHRA Detected?

      ↙        ↘
    NO          YES
    ↓            ↓
 Continue      Record Speech
 Listening         ↓
              ASR Server
                  ↓
             Transcription
📊 Performance

The repository contains model accuracy, testing and hardware results in the results/ directory.

Final real-world performance is being evaluated using the dedicated MEMS microphone dataset.
🔮 Future Improvements
*Larger speaker-diverse dataset
*Speaker-independent evaluation
*Long-duration false-activation testing
*Further latency optimization
*PCB implementation
*Compact enclosure
*Battery-powered operation
*Improved ASR integration
*Real-world environmental testing
