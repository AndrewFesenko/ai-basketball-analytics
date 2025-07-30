# 🏀 Analyzing UF's Championship Game with Computer Vision

After the University of Florida won the 2025 college basketball championship, Gainesville went wild. Students filled the streets, and my roommates and I couldn't stop rewatching the game. That energy led to this project — a computer vision system that analyzes basketball footage from real games.

This tool detects players and the ball, tracks possession, assigns teams based on jersey color, and even maps everything to a tactical top-down view of the court. It started as a way to study key plays from the UF win and turned into a full analysis pipeline.

---

## 🧠 What It Does

- 🧍 **Detects players and the ball** using YOLOv5/YOLOv8  
- 🎯 **Tracks movement** to calculate distance and speed for each player  
- 🧢 **Assigns teams** using a zero-shot image classifier based on jersey color  
- 🏀 **Logs passes and interceptions** by detecting possession changes  
- 📍 **Detects court keypoints** to understand player positioning  
- 📐 **Transforms perspective** to generate a tactical top-down view  
- 🎥 **Outputs an annotated game video** showing all tracked events and stats  

---

## ⚙️ Tech Stack

- **Python**
- **YOLOv5 / YOLOv8** – player, ball, and keypoint detection  
- **Roboflow** – dataset hosting and augmentation  
- **OpenCV + NumPy** – video frame processing and geometry  
- **Hugging Face Transformers** – zero-shot team classification  
- **Matplotlib** – drawing overlays and visualizations  
- **Docker (optional)** – containerized execution  

---

## 📁 Models and Datasets

This project uses several pretrained and custom-trained models:

- [ball_detector_model.pt](https://drive.google.com/drive/folders/1hckB1gdLNcbg_PF9sSTkrn0MpAYWGYXH?usp=drive_link)  
- [court_keypoint_detector.pt](https://drive.google.com/drive/folders/1hckB1gdLNcbg_PF9sSTkrn0MpAYWGYXH?usp=drive_link)  
- [player_detector.pt](https://drive.google.com/drive/folders/1hckB1gdLNcbg_PF9sSTkrn0MpAYWGYXH?usp=drive_link)

Additional resources:

- [Basketball detection dataset (Roboflow)](https://universe.roboflow.com/workspace)
- [Court keypoint dataset](https://universe.roboflow.com/fyp-3bw)
- [Zero-shot classifier (Hugging Face)](https://huggingface.co/patrickjohncyh)


## 🎥 Demo Video

Here are a few clips showing the system in action:

https://github.com/user-attachments/assets/ff8207c4-949c-4177-b304-23d74149e8a1


https://github.com/user-attachments/assets/2a8f8079-703d-4759-a31d-69d210fdb3e2


https://github.com/user-attachments/assets/e4b75d09-8099-4193-9ff0-08d1ff25e91b

