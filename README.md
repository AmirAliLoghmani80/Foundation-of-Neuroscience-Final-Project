# Foundation-of-Neuroscience-Final-Project

This project compares the object recognition performance of the HMAX model, which is inspired by the primate visual cortex, with human subjects. The focus of the study is to evaluate the strengths and limitations of the HMAX model through a series of experiments, comparing its performance to human participants using the same datasets.

## Project Overview

Object recognition is crucial for both artificial intelligence (AI) systems and human vision. This project aims to assess how well the HMAX model, which emulates hierarchical processing in the visual cortex, replicates human-like object recognition.

### Key Objectives

1. **Model Evaluation**: Evaluate the robustness, generalization, and speed of the HMAX model in object recognition tasks.
2. **Human Comparison**: Design and conduct human experiments to perform similar tasks and compare their performance to the HMAX model.
3. **Insights into AI and Neuroscience**: Contribute to the discourse on biologically inspired AI models and their capability to mirror human visual processing.

## Materials and Methods

- **HMAX Model**: The HMAX model is built upon multiple layers:
  - **S1 Layer**: Simulates simple cells using Gabor filters to capture basic visual patterns like edges.
  - **C1 Layer**: Pools responses from S1 to achieve invariance to small position and scale changes.
  - **S2 Layer**: Applies max-pooling to enhance selectivity for more complex patterns.
  - **C2 Layer**: Captures abstract representations of objects for robust recognition.
  - The model is trained using supervised learning, with the C2 layer outputs fed into an SVM classifier.

- **Behavioral Task Implementation**: Human participants were shown the same dataset as the HMAX model. Images were displayed for 20 milliseconds, and participants had to determine if the image contained an animal or not. A shuffled version of the image was presented to disrupt brain feedback mechanisms, creating parity with the HMAX model’s lack of feedback.

## Dataset

- The dataset consists of 1200 images, split evenly between animal and non-animal categories. Images were further divided into four subgroups:
  - **Head**
  - **Close Body**
  - **Medium Body**
  - **Far Body**

## Results

- **HMAX Model Results**: 
  - Head: 73.33%
  - Close Body: 78%
  - Medium Body: 74.67%
  - Far Body: 68%
  - **Average Accuracy**: 73.5%

- **Human Subjects**: 
  - Testing was conducted with 3 individuals, and their performance surpassed the HMAX model across all categories.

### Conclusion

While the HMAX model shows reasonable performance in object recognition tasks, human subjects outperform the model across all image categories. However, the results suggest that combining different models or improving feature extraction techniques could enhance the HMAX model’s performance.

## Figures

- **ROC Curve**: Provided for the test set.
- **Confusion Matrix**: Showing classification results for the HMAX model.
- **Comparison of Accuracies**: For different image categories between the HMAX model and human subjects.

## Instructions for Use

1. **HMAX Model Implementation**: Follow the provided code to implement the HMAX model with the given dataset.
2. **Human Experiment**: Replicate the human experiment by displaying the images to subjects and recording their responses.

## Conclusion

This study provides a comparative analysis between a biologically inspired AI model and human vision in object recognition tasks. The findings suggest that while the HMAX model is effective, there is still a significant gap between AI models and human capabilities in visual processing tasks.
