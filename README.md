# ECG Heartbeat Classification using LSTM
## Project Overview
This project employs Long Short-Term Memory (LSTM) networks to analyze electrocardiogram (ECG) data, aiming to detect R-peaks and classify heartbeat normality. Leveraging the MIT-BIH Arrhythmia Database, it seeks to enhance heart condition diagnostics through advanced machine learning techniques.

## Objectives
- Apply LSTM networks for precise R-peak detection.
- Classify heartbeat normality to identify potential cardiac issues.
- Address the challenges posed by class imbalance in medical datasets.

## Dataset and Bias Consideration
The dataset comprises ECG recordings (MLII and V5 leads) and annotations detailing R-peaks and heartbeat types. A significant challenge identified is the class imbalance due to a disproportionate ratio of labeled versus unlabeled data. This imbalance could lead to overestimated accuracy for the majority class, misrepresenting the model's actual performance. To mitigate this, the project emphasizes the importance of using balanced datasets and evaluation metrics like precision-recall analysis.

## Model Architecture
The model leverages LSTM layers to capture the temporal dependencies within ECG time-series data effectively. With dual outputs, the model predicts R-peaks and classifies heartbeat normality. It includes:

- An LSTM layer for learning sequential data characteristics.
- A Dense layer with a sigmoid activation function for R-peak detection.
- A Dense layer with a softmax activation function for heartbeat normality classification.

## Technologies Used
- Python
- TensorFlow and Keras for model building and training.
- Pandas and NumPy for data manipulation.
- Matplotlib for data visualization.

## Results
Despite potential bias from class imbalance, initial results are promising. The model demonstrates competence in detecting R-peaks and classifying heartbeat normality. Ongoing efforts are directed toward refining evaluation metrics to accurately reflect the model's effectiveness.
