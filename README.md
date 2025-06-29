## 🦺 Construction Worker Safety Gear Detection — YOLOv8

This project uses **YOLOv8** to detect construction workers and check if they’re wearing required safety gear like **helmets** and **safety vests** in real-time video feeds or images.


## 🏋️‍♂️ How to Train a Custom Model

1. Prepare your dataset in YOLO format:

   ```
   dataset/
   ├── images/
   │   ├── train/
   │   ├── val/
   ├── labels/
   │   ├── train/
   │   ├── val/
   ```

2. Update your `yolov8_config.yaml` with paths and class names (`jacket`, `hat`).

3. Run training:

   ```bash
   yolo detect train data=yolov8_config.yaml model=yolov8n.pt epochs=100 imgsz=640
   ```

---

## ⚙️ Requirements

* Python 3.8+
* [Ultralytics YOLOv8](https://docs.ultralytics.com/)
* OpenCV
* PyTorch

Install with:

```bash
pip install ultralytics opencv-python
```

---

## ✅ Features

* Detects construction workers’ helmets and vests.
* Supports images, videos, and real-time webcam.
* Uses state-of-the-art YOLOv8 model.
* Easy to retrain with your own dataset.

---

## 📃 License

MIT License.
Feel free to use, share, or adapt!

---

## 🤝 Credits

Built with [YOLOv8](https://github.com/ultralytics/ultralytics) and [OpenCV](https://opencv.org/).

