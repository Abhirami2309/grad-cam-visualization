# Grad-CAM: Visualizing CNN Decisions

This project implements **Gradient-weighted Class Activation Mapping (Grad-CAM)** to visually explain the decision-making process of a pre-trained **ResNet50** model. Grad-CAM generates class-specific heatmaps that highlight the salient regions in an image that most influence the model's prediction.

---

## Method

The Grad-CAM heatmap is generated through the following steps:

1. **Compute Gradients**: Calculate the gradients of the predicted class score with respect to the feature maps of the final convolutional layer.
2. **Weight Feature Maps**: Use the gradients as weights to compute a weighted sum of the feature maps.
3. **Generate Heatmap**: The result is a heatmap that highlights the important regions in the input image influencing the model’s decision.

---

## Usage & Dependencies

### Install Required Libraries

Run the following command to install dependencies:

```bash
pip install torch torchvision opencv-python matplotlib requests
