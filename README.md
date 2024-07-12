# Project Name: Painter Recognition

<div align="center">
  <img src="art_recognition.jpg" alt="Painting Classification">
</div>

## Overview

The goal of this project is to develop a model capable of recognizing paintings from three different painters: Caravaggio, Manet, and Van Gogh. The images may vary in style, pose, genre, and may include backgrounds, frames, or occlusions. The focus is on building a robust dataset, training a model that generalizes well, and iteratively improving the model through alternate training and validation processes.

## Dataset

- **Coverage:** Ensure the dataset covers the production of each painter as comprehensively as possible.
- **Generalization:** Train the model to classify images not included in the training set.
- **Robustness:** Develop a model that is not affected by frames, backgrounds, occlusions, etc.

## Model Training and Validation

- **Iterative Process:** Model training and validation are not a one-time feed-forward process.
- **Sample Analysis:** After each validation, analyze misclassified samples to understand and address issues.
- **Adaptations:** Modify the model or training set based on analysis to improve performance.
- **Challenge Validation Set:** Ensure the validation set is challenging enough to validate the model's true performance.
- **Documentation:** Keep track of countermeasures and improvements for the final project presentation.

## Implementation Details

### Tools and Requirements

- **Algorithms:** Any classifier, including non-neural ones.
- **Explanation:** Provide clear explanations for algorithms, preprocessing, training strategy, and validation.
- **Google Colab:** Code must be runnable inside Google Colab.
- **Data Augmentation:** Utilize data augmentation techniques.
- **Local Computing:** Use local computing power for training (not limited to Colab).

## Submission Requirements

Submit a Google Colab Notebook containing:

1. **Code to Load Trained Model**
2. **Predict Function:**

   - **Prototype:** `predict(X)`
   - **X (Input):** Tensor containing a batch of test samples with shape `(batch_size, rows, cols, 3)` of type `uint8`.
   - **Return Value:** Tensor with predictions on the batch in one-hot encoding, with shape `(batch_size, 3)`.
   - **Classes Order:** 1. Caravaggio, 2. Manet, 3. Van Gogh.
   - **Function Independence:** The function should work independently of the batch size.
   - **Preprocessing and Postprocessing:** Perform all required preprocessing on the test data batch and postprocessing on the results before returning them.

## Folder Organization

- **UltimateDataSet2.0/**: Contains the comprehensive dataset used for training and validation.
- **final_log/**: Logs and records of the training and validation processes.
- **final_model/**: The final trained model ready for deployment.
- **FinalPresentationMachineLearning.pptx**: Presentation summarizing the project and its results.
- **FinalProjectMachineLearning.pdf**: Final report detailing the project, methodologies, and outcomes.
- **README.md**: This README file providing an overview of the project.
- **test.ipynb**: Jupyter notebook for testing the model and making predictions.
- **train.ipynb**: Jupyter notebook for training the model.

## Conclusion

This README provides an overview of the Painter Recognition project, including dataset considerations, model training and validation strategies, and implementation details. Please refer to the accompanying Google Colab Notebook for the complete code and functionality.
