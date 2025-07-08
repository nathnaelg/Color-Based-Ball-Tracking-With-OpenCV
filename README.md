## 📌 Project Overview

**Color-Based Ball Tracking With OpenCV** is a computer vision project that uses color segmentation to track the movement of balls in a video. It detects the color of each ball, determines its position in frame quadrants, logs entry and exit times, and generates an annotated output video showing tracking details.

---

## 🎥 Demo & Files

- **Input Video**: `AI Assignment video.mp4`
- **Output Video**: `processed_video.avi`
- **Event Log**: `events.csv`

The output video contains overlays indicating the ball's position, direction, and quadrant transitions. All events are timestamped and saved for review in the CSV file.

---

## 🗂️ Project Structure

```

📁 Color-Based-Ball-Tracking-With-OpenCV/
├── .gitattributes                  # Git settings
├── AI Assignment video.mp4        # Input video file for tracking
├── LICENSE                        # License file (MIT)
├── README.md                      # Project documentation
├── events.csv                     # Output log of events (entry/exit times)
├── processed\_video.avi            # Annotated output video
└── trani model.ipynb              # Main Jupyter notebook (typo: 'trani' → 'train' or 'tracking')

````

---

## ⚙️ Installation

### 1. Clone the repository

```bash
git clone https://github.com/your-username/Color-Based-Ball-Tracking-With-OpenCV.git
cd Color-Based-Ball-Tracking-With-OpenCV
````

### 2. Install dependencies

Make sure you have Python 3.7+ and Jupyter installed. Then run:

```bash
pip install opencv-python numpy imutils
```

Or install from within the notebook.

---

## 🚀 Getting Started

1. Open the Jupyter notebook:

```bash
jupyter notebook "trani model.ipynb"
```

2. Run the cells in sequence:

   * Load and preprocess the video
   * Apply HSV-based color masking
   * Detect ball contours and calculate positions
   * Log entry/exit events based on quadrant transitions
   * Write results to `processed_video.avi` and `events.csv`

3. Review the output files in the root directory.

---

## 📊 Sample Event Log (`events.csv`)

| Timestamp   | Color | Event   | Quadrant |
| ----------- | ----- | ------- | -------- |
| 00:00:05.12 | Red   | Entered | Q1       |
| 00:00:06.45 | Red   | Exited  | Q2       |
| 00:00:07.21 | Green | Entered | Q3       |

---

## 🧪 Features

* 🎯 **Color Detection** using HSV thresholding
* 🧭 **Quadrant Detection** in a 2x2 frame split
* 📝 **Event Logging** (entry & exit per quadrant)
* 🎥 **Processed Video Output** with overlays

---

## 🛠️ Customization

You can easily customize the project:

* 🎨 Change tracked colors by modifying HSV ranges
* 📐 Adjust quadrant logic to fit other layouts
* 🖼️ Change video resolution or format
* 📄 Log additional metrics like speed or trajectory

---

## 📚 Use Cases

* 🏀 Sports video analysis
* 🤖 Robotics vision systems
* 🎓 Educational demos for OpenCV and tracking
* 📹 Surveillance and area monitoring

---

## 🤝 Contributing

Feel free to fork this repo and submit pull requests.
For any major changes, please open an issue first.

---

## 📜 License

This project is licensed under the MIT License. See the `LICENSE` file for details.

---

## ✏️ Notes

* The file name `trani model.ipynb` contains a typo. Consider renaming it to `tracking_model.ipynb` for clarity.
* You can convert this notebook to a Python script using:

```bash
jupyter nbconvert --to script "trani model.ipynb"
```

---

> Created with ❤️ using Python & OpenCV

```
