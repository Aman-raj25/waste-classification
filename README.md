# Waste Classification Using Deep Learning: A Comparative Analysis

## Overview

This project presents a **comparative analysis** of different deep learning models for automated waste classification. Efficient waste sorting is crucial for recycling and sustainability, but traditional methods are slow and error-prone. Deep learning offers a scalable solution by automating classification with high accuracy.

We compare a **custom CNN** with three pre-trained models—**ResNet50, MobileNetV3, and EfficientNetB3**—to determine the best approach for real-world deployment.

## Features

- **Automated Waste Classification**: Classifies waste into five categories—plastic, paper, glass, organic, and textile.
- **Model Comparison**: Evaluates accuracy, computational efficiency, and deployment feasibility.
- **Dataset Processing**: Standardizes images and applies preprocessing techniques.
- **Performance Metrics**: Uses accuracy, precision, recall, and F1-score for model evaluation.

## Dataset

The dataset consists of **1,987 labeled images** categorized into five waste types. Images are preprocessed to ensure uniform resolution (**224×224 pixels**) and RGB format. Stratified sampling is used to maintain class balance across training and validation sets.

### Dataset Distribution:
- **Plastic**: 20%
- **Paper**: 20%
- **Glass**: 20%
- **Organic**: 18%
- **Textile**: 22%

## Installation

Ensure you have the following dependencies installed:
```bash
pip install tensorflow numpy pandas matplotlib pillow
```

## Usage

1. Clone the repository:
   ```bash
   git clone https://github.com/Aman-raj25/waste-classification.git
   ```
2. Navigate to the project directory:
   ```bash
   cd waste-classification
   ```
3. Run the Jupyter Notebook to preprocess data, train models, and evaluate performance.

## Model Comparisons

We implemented and tested four models to determine their effectiveness in waste classification:

| Model         | Accuracy | Precision | Recall | F1-Score | Best Use Case |
|--------------|----------|-----------|--------|----------|---------------|
| **Custom CNN** | 76.2%   | 76.4%     | 75.8%  | 75.0%    | Basic feature extraction |
| **ResNet50**  | 96.2%   | 95.8%     | 96.2%  | 96.0%    | High-accuracy applications |
| **MobileNetV3** | 92.7%   | 92.8%     | 93.5%  | 93.0%    | Mobile & edge devices |
| **EfficientNetB3** | 91.4% | 91.0% | 92.3% | 92.8% | Cloud-based systems |

### Model Insights:
- **Custom CNN**: Lightweight but struggles with feature extraction, leading to misclassifications.
- **ResNet50**: Best overall accuracy but computationally expensive.
- **MobileNetV3**: Balanced trade-off between speed and accuracy, making it ideal for edge deployment.
- **EfficientNetB3**: Slightly less accurate than MobileNetV3 but optimized for cloud-based systems.

## Results & Observations

- **ResNet50** had the highest accuracy (96.2%), making it ideal for high-performance applications.
- **MobileNetV3** is the best option for real-time classification in **mobile or IoT applications**.
- **EfficientNetB3** balances accuracy and computational efficiency, making it ideal for **cloud-based AI**.
- **Custom CNN**, while foundational, struggled with misclassifications and had the lowest performance.

## Future Enhancements

- **Hybrid AI Models**: Combining CNNs with Vision Transformers (ViTs) for enhanced feature extraction.
- **Smart Waste Sorting**: Deploying models in real-time waste classification systems.
- **Edge AI Integration**: Optimizing models for deployment on Jetson Nano and Raspberry Pi.

## Contributing

Contributions are welcome! You can help by improving the dataset, optimizing model performance, or integrating real-world deployment solutions.

## License

This project is open-source and available under the MIT License.
