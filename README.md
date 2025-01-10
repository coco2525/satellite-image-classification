# Satellite Image Classification System

## Project Overview
This project focuses on classifying satellite images into predefined categories using various machine learning techniques. The model predicts and categorizes images into **cloudy**, **desert**, **forest**, and **water** categories based on visual features. It demonstrates the practical applications of satellite image analysis in fields like environmental conservation and agriculture.

---

## Key Features
- **Data Source**: [Satellite Image Classification Dataset](https://www.kaggle.com/datasets/mahmoudreda55/satellite-image-classification)
- **Categories**:
  - Cloudy
  - Desert
  - Forest
  - Water
- **Preprocessing**:
  - Resized images to 100x100 pixels.
  - Converted CMYK images to RGB.
  - Extracted features using RGB averages, grayscale, LBP, and Prewitt edge detection.
- **Machine Learning Models**:
  - Logistic Regression, Naive Bayes, Decision Trees, Random Forests, SVM (Linear, RBF, Polynomial, Sigmoid), K-Nearest Neighbor.
- **Deployment**:
  - A web application for real-time classification: [Try it here](https://coco2525.pythonanywhere.com/image_classification)

---

## Data and Analysis

### Preprocessing
- **Dataset**: 1421 images sampled to fit Google Colab's RAM limitations.
- **Feature Engineering**:
  - RGB conversion, grayscale transformation.
  - LBP (Local Binary Pattern) feature extraction.
  - Prewitt filter for edge detection.

### Visualization
- **Category Distribution**: Bar chart showing dataset balance across categories.
- **Sample Images**: Visual validation of representative images from each category.
- **RGB Layers**:
  - Desert and cloudy images showed uniform color distribution.
  - Forest images highlighted strong green tones.
  - Water images emphasized blue-green patterns.
- **Edge Patterns**:
  - Prewitt edge detection visualized unique edge characteristics for each category.

---

## Model Performance

### Cross-Validation Accuracy (fig.5):
| Model                | Accuracy (%)     |
|----------------------|------------------|
| Random Forest        | 88.63 ± 3.29    |
| Linear SVM           | 82.49 ± 3.64    |
| Logistic Regression  | 80.88 ± 3.04    |
| RBF SVM              | 25.06           |

### Test Data Performance (fig.6):
| Model                | Accuracy (%)     |
|----------------------|------------------|
| Random Forest        | 87.82           |
| Linear SVM           | 84.31           |
| Logistic Regression  | 78.92           |

---

## Deployment
- The model is deployed as a web application, allowing users to upload an image and classify it instantly.
- **Web Application**: [Satellite Image Classifier](https://coco2525.pythonanywhere.com/image_classification)

---

## Applications
1. **Environmental Conservation**:
   - Monitor deforestation and desertification.
   - Detect water pollution and marine health.
2. **Agriculture**:
   - Monitor crop health and growth.
   - Optimize irrigation and fertilization schedules.
   - Detect crop diseases and pest damage.

---

## Future Enhancements
- Expand the dataset to include regional and seasonal variations.
- Integrate long-term data for modeling climate trends.
- Extend classification to a global scale for worldwide environmental monitoring.

---

## Author
- **Momo Ogawa**
