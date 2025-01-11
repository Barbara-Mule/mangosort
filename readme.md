# MangoSort - A YOLOv8-Powered Mango Classification and Grading Mobile Application

## Project Overview
This is a YOLOv8-powered mango classification and grading system developed to assist farmers in Kenya to identifying Kenyan mango varieties and grading them based on quality standards. The system leverages deep learning models for image classification and object detection, integrated into a streamlined pipeline for training, evaluation, and deployment.

## Project Features
1. **Classification**: Identifies 9 distinct Kenyan mango varieties based on visual features.
2. **Grading**: Categorizes mangoes into three quality grades (Extra Grade, First Grade, Second Grade).
3. **Training and Evaluation**: Uses labeled datasets for training YOLOv8 models with performance metrics such as accuracy, precision, recall, and F1 score.
4. **Deployment**: Converts trained models to TensorFlow Lite format for efficient deployment.
5. **User-Friendly Mobile Interface**: Allows farmers to capture images of mangoes for automated analysis.
6. **Real-Time Feedback**: Provides immediate classification and grading results.

## Dataset Description
### **Classification Dataset**
- **Classes**: 9 mango varieties (e.g., Apple Mango, Boribo, Kent, Ngowe).
- **Total Images**: 1,800 (200 images per class).
- **Label Format**: Each image is labeled with a class index (0-8) and dummy bounding box coordinates for YOLO compatibility.

### **Grading Dataset**
- **Classes**: Extra Grade, First Grade, Second Grade.
- **Total Images**: 658 (202, 229, and 227 images, respectively).
- **Label Format**: Each image is labeled with a grade index (0-2) and dummy bounding box coordinates.

## Development Tools
- **Programming Language**: Python and Android
- **Frameworks**: Ultralytics YOLOv8, TensorFlow Lite
- **Integrated Development Environment (IDE)**: VS Code
- **Database Management**: Firebase
- **Version Control**: Git and GitHub
- **Prototyping Tools**: Figma

## System Requirements
### **Hardware Specifications**
- Processor: Intel Core i7 or equivalent
- RAM: 16 GB
- Storage: 50 GB free space
- GPU: NVIDIA GTX 1080 or higher (optional for training)

### **Software Specifications**
- Operating System: Windows 10 / Ubuntu 20.04
- Python Version: 3.8 or above
- Required Libraries: `ultralytics`, `tensorflow`, `numpy`, `sklearn`, `matplotlib`

## Model Training and Testing
- **Training Split**: 70% of the dataset is used for training.
- **Validation Split**: 15% of the dataset is used for validation.
- **Testing Split**: 15% of the dataset is reserved for testing.
- **Evaluation Metrics**: Accuracy, Precision, Recall, Mean Average Precision(mAP), F1 Score, and Confusion Matrix.

## Installation and Setup
1. Clone the repository:
   ```bash
   git clone <repository-url>
   ```
2. Install required dependencies:
   ```bash
   pip install -r requirements.txt
   ```
3. Extract the datasets:
   - Place the datasets in the `Dataset/Classification_dataset` and `Dataset/Grading_dataset` directories.
4. Run the training script:
   ```bash
   python yolov8_training.ipynb
   ```

## Usage
1. Launch the mobile application.
2. Capture images of mangoes using the device's camera.
3. View real-time classification and grading results on the application.

## System Architecture
- **External Entities**: Farmer, System Admin.
- **Core Components**: Mobile application, YOLOv8 models, and SQLite database.
- **Data Flow**:
  - Images are captured via the mobile app.
  - YOLOv8 models classify and grade the mangoes.
  - Results are stored in the database and displayed to the user.

## Future Enhancements
1. Extend the dataset to include more mango varieties and quality grades.
2. Optimize the YOLOv8 model for better performance on mobile devices.
3. Implement multilingual support for the mobile application.

## Contributions
Contributions to the project are welcome! Please fork the repository and submit a pull request with your changes.

## Contact
For inquiries, contributions, or feedback, please reach out to:
- **Name**: [Rachael Mule]
- **Email**: [rachael.mule@strathmore.edu]


Thank you for exploring the MangoSort!
