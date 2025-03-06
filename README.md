# Brain-tumor-detection



## The results.csv file has the following metrics for easier compilation of results

### **Training Metrics:**
1. **`epoch`** – The current training iteration (i.e., how many times the model has gone through the entire dataset).
2. **`train/box_loss`** – The loss related to bounding box regression (how well the model is predicting object locations).
3. **`train/cls_loss`** – The classification loss (how well the model is identifying object classes).
4. **`train/dfl_loss`** – The Distribution Focal Loss (DFL) used to improve bounding box localization.

### **Validation Metrics:**
5. **`metrics/precision(B)`** – The proportion of positive detections that are correct (how precise the model is).
6. **`metrics/recall(B)`** – The proportion of actual objects correctly detected (how many true positives the model finds).
7. **`metrics/mAP50(B)`** – The mean Average Precision (mAP) at 50% IoU (Intersection over Union), a standard metric for object detection.
8. **`metrics/mAP50-95(B)`** – The mean Average Precision across different IoU thresholds (50% to 95%), providing a more comprehensive evaluation.

### **Validation Losses (After Each Epoch):**
9. **`val/box_loss`** – The validation loss for bounding box regression.
10. **`val/cls_loss`** – The validation loss for classification.
11. **`val/dfl_loss`** – The validation loss for Distribution Focal Loss.

### **Learning Rates:**
12. **`lr/pg0`**, **`lr/pg1`**, **`lr/pg2`** – Learning rates for different parameter groups, which help track how the optimizer adjusts learning rates over time.
