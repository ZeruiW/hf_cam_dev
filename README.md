# XAI Service Documentation

---

## 1. XAI Service

- **Directory**: `xai`
- **Purpose**: Provides XAI (Explainable Artificial Intelligence) service.
- **Details**:
  - Implements various CAM (Class Activation Mapping) methods for different models.
  - Utilizes the `ImageNet-Mini` dataset as input for the analysis.(structure constant for other datasets)
  - Currently, the XAI explanations are generated and stored in the `results` folder. should send to database.

---

## 2. Feature Transformation
- **Directory**: `feature transform`
- **Notebook**: `masking`
- **Purpose**: To transform XAI results into masking images.
- **Details**:
  - Reads from the `results` directory.
  - Processes the XAI results and generates masking images.
  - Masking images are stored in the `evaluation` folder.

---

## 3. Prediction Changes Evaluation

- **Directory**: `prediction_changes`
- **Notebook**: `pcd.ipynb`
- **Purpose**: Evaluates the impact of the feature transformations.
- **Details**:
  - Reads from the `evaluation` directory.
  - Calculates prediction changes scores based on the masked images.
  - Provides a comprehensive statistical analysis of the results.

