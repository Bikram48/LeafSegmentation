### Leaf Segmentation and Quantification

This project focuses on leaf segmentation and counting using deep learning models. It employs **ResNet-UNet** for semantic segmentation (5 classes: background + 4 leaf types) and **ResNet-50** for leaf counting.

---

### Dataset

- **Images**: 200 campus images of fallen leaves.
- **Classes**: Eastern Cottonwood, Sugar Maple, Camellia, River Birch.
- **Annotations**: Masks created using the VIA tool.

---

### Preprocessing

- **Data augmentation**: Random resizing, flipping, rotation, color adjustments, and Gaussian blur.
- **Image dimensions**: Resized to 224x224.
- **Normalization**: Mean=[0.4829, 0.4384, 0.3892], Std=[0.2369, 0.2155, 0.2078].
- **Dataset split**: 80% training, 10% validation, 10% testing.

---

### Models

- **ResNet-UNet**: Used for semantic segmentation to classify each pixel into one of the 5 classes.
- **ResNet-50**: Fine-tuned for regression to predict the number of leaves in an image.

---

### Results

- **Segmentation accuracy**: Achieved a training accuracy 74.85% and test accuracy 74.30%
- **Counting accuracy**: Mean Absolute Error (MAE) of [your metric here].

---

### Future Work

- Extend the dataset with more leaf types and diverse environments.
- Incorporate real-time detection capabilities.

---
