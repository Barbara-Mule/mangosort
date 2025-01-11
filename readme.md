#IS Project II
# MangoSort - A Mango Classification and Grading System

This is a YOLOv8-powered mango classification and grading system to assist farmers in Kenya to identifying Kenyan mango varieties and grading them based on quality standards. The system leverages deep learning models for image classification and object detection, integrated into a streamlined pipeline for training, evaluation, and deployment.

## Project Features
- **Classification**: Identifies 9 distinct Kenyan mango varieties based on visual features.
- **Grading**: Categorizes mangoes into three quality grades (Extra Grade, First Grade, Second Grade).
- **Training and Evaluation**: Uses labeled datasets for training YOLOv8 models with performance metrics such as accuracy, precision, recall, and F1 score.
- **Deployment**: Converts trained models to TensorFlow Lite format for efficient deployment.

## Dataset Description
### Classification Dataset
- **Classes**: 9 Kenyan mango varieties
- **Total Images**: 1,800 (200 images per variety)
- **Split**:
  - 70% Training
  - 15% Validation
  - 15% Testing

### Grading Dataset
- **Classes**: Extra Grade, First Grade, Second Grade
- **Total Images**: 658
  - Extra Grade: 202 images
  - First Grade: 229 images
  - Second Grade: 227 images
- **Split**:
  - 70% Training
  - 15% Validation
  - 15% Testing

## Project Structure
```
project/
├── classification_dataset/        # Raw classification dataset
├── grading_dataset/               # Raw grading dataset
├── output/                        # Processed datasets and results
│   ├── Classification_Dataset/
│   ├── Grading_Dataset/
├── scripts/                       # Python scripts for training and evaluation
├── models/                        # Trained YOLOv8 models
├── README.md                      # Project documentation
```

## Setup and Installation
1. **Clone the Repository**:
   ```bash
   git clone <repository-url>
   cd project
   ```

2. **Install Dependencies**:
   ```bash
   pip install ultralytics tensorflow numpy sklearn
   ```

3. **Prepare the Dataset**:
   - Extract the datasets to their respective directories.
   - Ensure proper folder structure for classification and grading datasets.

4. **Run Dataset Preparation**:
   ```bash
   python scripts/prepare_datasets.py
   ```

5. **Train the Models**:
   - Classification Model:
     ```bash
     python scripts/train_classification.py
     ```
   - Grading Model:
     ```bash
     python scripts/train_grading.py
     ```

6. **Evaluate the Models**:
   ```bash
   python scripts/evaluate_models.py
   ```

7. **Deploy the Models**:
   ```bash
   python scripts/export_to_tflite.py
   ```

## Key Components
### YOLOv8 Models
- **Framework**: Ultralytics YOLOv8
- **Classification Task**: Predicts mango variety
- **Grading Task**: Detects and grades mangoes based on quality

### Tools and Technologies
- **Programming Language**: Python
- **Frameworks**: YOLOv8, TensorFlow
- **Metrics**: Accuracy, Precision, Recall, F1 Score
- **Deployment**: TensorFlow Lite

## Contributions
Contributions to the project are welcome! Please fork the repository and submit a pull request with your changes.

## License
This project is licensed under the MIT License. See the `LICENSE` file for more details.

## Contact
For inquiries or feedback, contact:
- **Email**: rachael.mule@strathmore.edu
- **GitHub**: [Your GitHub Profile](https://github.com/yourprofile)

---

Thank you for exploring the Mango Classification and Grading System!
