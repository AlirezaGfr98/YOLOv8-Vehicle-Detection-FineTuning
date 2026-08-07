# 🚗 Vehicle Detection Using YOLOv8

This project fine-tunes three versions of YOLOv8 (Small, Medium, Large) on a custom vehicle detection dataset. The dataset includes images of vehicles from traffic scenes and is augmented to improve model generalization.

## 📁 Dataset
- Classes: `truck`, `bus`, `car`, `bicycle`, `motorbike`
- Images: 105 total (split into train/val/test)

## 🧠 Models
- YOLOv8s
- YOLOv8m
- YOLOv8l

All models are fine-tuned using:
- Data augmentation (mosaic, flip, HSV, scaling, translation)
- AdamW optimizer
- Cosine learning rate scheduler
- 50 epochs

## 📊 Results

| Model     | Precision | Recall | mAP@0.5 | mAP@0.5:0.95 |
|-----------|-----------|--------|---------|---------------|
| YOLOv8s   | 0.3459    | 0.4810 | 0.4902  | 0.3312        |
| YOLOv8m   | 0.7653    | 0.2573 | 0.3662  | 0.2053        |
| YOLOv8l   | 0.6913    | 0.2562 | 0.2699  | 0.1781        |

> The YOLOv8s model shows the best balance between mAP and recall.

## 🧪 How to Run
1. Open `Task_5.ipynb` in Google Colab.
2. Mount Google Drive.
3. Run all cells to train, validate, and test the models.

## 📈 Visualizations
- mAP comparison chart
- Sample predictions from test images

## 📦 Requirements
- ultralytics
- wandb
- opencv-python
- matplotlib
- pandas
- Pillow

## 🔗 Links
- [Weights & Biases Dashboard](https://wandb.ai/alighaffari1234567-academy-hamrah/Vehicle-Detection-YOLOv8)
