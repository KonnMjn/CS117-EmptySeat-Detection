# 💺 Empty Seat Detection in Coffee Shops

A Computational Thinking Project Proposal for detecting available seats in a coffee shop environment using video stream analysis and object detection.

---

## 📌 Table of Contents

- [Project Overview](#project-overview)
- [Computational Thinking Breakdown](#compuational-thinking-breakdown)
- [Project Structure](#project-structure)
- [Dataset](#dataset)
- [Methodology](#methodology)
- [How to Run](#how-to-run)
- [Notes](#notes)
- [License](#license)
- [Credits](#credits)

---

## 📚 Project Overview

This project applies **Computational Thinking** principles — Abstraction, Decomposition, Pattern Recognition, and Algorithm Design — to design a system that identifies the number of empty seats in a coffee shop using real-time camera footage.

The project does not include implementation code but provides a detailed theoretical and design-based solution.

---

## 👀 Computational Thinking Breakdown

- **Abstraction**: Ignore unnecessary visual details, focus only on chair occupancy detection.
- **Decomposition**: Split the problem into modules such as preprocessing, object detection, occlusion filtering, thresholding, and result aggregation.
- **Pattern Recognition**: Apply common computer vision workflows: preprocessing → detection → filtering → classification.
- **Algorithm Design**: Flowchart outlines detection pipeline from input video to output result.

---

## 📁 Project Structure

```
EmptySeat-Detection/
├── Project Poster.pdf
├── Project Report.docx
├── Algorithm-Flowchart.png
├── Decomposition-Tree.drawio.png
├── README.md
├── .gitignore
```
---

## 📦 Dataset

| Dataset Name      | Source             | Use                      |
|-------------------|--------------------|--------------------------|
| ImageNet VID/DET  | External datasets  | Training object detector |
| OVIS              | Video Segmentation | Classification           |
| Real Cafe Videos  | Simulated          | Seat status labeling     |

The above data sets are for reference only and have not been actually applied to the topic.

---
## 🧠 Methodology

1. **Input**: Video streams from top-down cameras placed over table rows.
2. **Preprocessing**: Filter out occluded frames (≥25% chairs blocked).
3. **Object Detection**: Apply YOLO or similar model to detect chairs.
4. **Occupancy Check**: For each chair, classify it as “empty” or “occupied”.
5. **Threshold Rule**: If 90% of recent 5-min frames detect a chair as empty → it is empty.
6. **Output**: Total number of empty seats, returned within ≤7 seconds.

--- 

## 🚀 How to Run

> This repository is meant for **conceptual reference**. No executable code is provided.

1. Review `/docs/Project Report.pdf` for full analysis.
2. Open `/docs/Project Poster.pdf` for a quick summary.

---

## 📌 Notes
This repo includes only manually added data and annotations.

Original dataset must be downloaded from Kaggle.

Make sure to update paths in main.ipynb if using different folder structures.

--- 

## 📄 License
This project is for educational purposes. Feel free to use, modify, and distribute with attribution.

---

## 👨‍🏫 Credits

Đinh Tuệ Đức - 22520263 

Phạm Đông Hưng – 22520521

Lương Anh Huy - 22520550

Phan Công Minh - 22520884

Hồng Khải Nguyên - 22520967

Instructor: TS. Ngô Đức Thành

---
