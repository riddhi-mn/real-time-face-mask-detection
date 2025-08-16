Comparative analysis of three convolutional neural network (CNN) architectures - tailored for real-time face mask detection. 

<h2> Models Compared: </h2>
1)ResNet50 – deeper model, fine-tuned with unfrozen layers.
2)MobileNetV2 – lightweight, depthwise separable convolutions, trained head-only.
3)EfficientNetB0 – fully fine-tuned with compound scaling.

Dataset used : “Omkargurav/face-mask-dataset” from Kaggle, containing 7,553 RGB face images — 3,725 with masks and 3,828 without.

Overall metrics achieved:
| Model              | Accuracy | Precision | Recall    | F1-Score  | Notes                                                 |
| ------------------ | -------- | --------- | --------- | --------- | ----------------------------------------------------- |
| **MobileNetV2**    | **98%**  | 0.99      | 0.98      | 0.98–0.99 | Best for edge devices (fast + lightweight).           |
| **EfficientNetB0** | 97%      | 0.95–0.99 | 0.95–0.99 | 0.97      | Strong generalization, slightly heavier.              |
| **ResNet50**       | 94%      | 0.94      | 0.94      | 0.94      | High capacity, but less efficient for small datasets. |




