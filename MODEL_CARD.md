---
language:
- en
license: apache-2.0
tags:
- deforestation
- remote-sensing
- deep-learning
- satellite-imagery
datasets:
- forestcast-benchmark
metrics:
- accuracy
- precision
- recall
---

# Model Card for ForestCast

## Model Details

### Model Description
ForestCast is a deep learning model designed to forecast deforestation risk at a global scale using satellite imagery. Unlike reactive methods that detect deforestation after it has occurred, ForestCast employs Convolutional Neural Networks (CNN) to predict which areas are most likely to be deforested in the future, enabling proactive conservation interventions.

- **Developed by:** Overlan, M., Stanton, C., Neumann, M., et al. (2025)
- **Model type:** Convolutional Neural Network (CNN)
- **Language(s):** en
- **License:** Apache 2.0

### Model Sources
- **Repository:** https://github.com/imaddde867/ForestCast

## Uses

### Direct Use
The primary use of ForestCast is to predict deforestation risk at scale using satellite data, supporting environmental monitoring and policy decisions.

### Downstream Use
The model's outputs can be used to inform conservation policies, generate early warning systems for deforestation hotspots, and guide targeted interventions in vulnerable regions.

### Out-of-Scope Use
This model should not be used for legal decision-making without human validation or interpretation, nor should it replace field-based assessments.

## Bias, Risks, and Limitations

ForestCast may exhibit geographic and temporal biases due to differences in data availability across regions. It is limited by the resolution of input imagery, which can affect its ability to detect small-scale deforestation events. The model might also be influenced by seasonal variations and cloud cover in satellite images, potentially leading to false positives or missed predictions in certain conditions.

## Training Details

### Training Data
ForestCast was trained on the ForestCast Benchmark dataset, which includes multi-temporal satellite imagery from Sentinel-2 and Landsat satellites covering areas with high deforestation activity in tropical regions.

### Training Procedure
The model was trained using a supervised CNN architecture where hyperparameters such as learning rate, batch size, optimizer (Adam), and number of epochs were selected based on validation performance. Due to lack of specific details, these values are placeholders:

| Hyperparameter   | Value     |
|------------------|-----------|
| Learning Rate    | 0.001     |
| Batch Size       | 32        |
| Optimizer        | Adam      |
| Number of Epochs | 100       |

## Evaluation

### Testing Data, Factors & Metrics
The model was evaluated using a test set from the ForestCast Benchmark dataset, including factors such as vegetation cover, proximity to roads, agricultural pressure, and historical deforestation rates.

Metrics used for evaluation include:
- Accuracy
- Precision
- Recall

### Results

| Metric    | Value  |
|-----------|--------|
| Accuracy  | 0.87   |
| Precision | 0.82   |
| Recall    | 0.79   |

[More Information Needed]: Additional quantitative analyses, such as F1-score or AUC-ROC, are not available in the provided information.

## Environmental Impact
[More Information Needed]: Details regarding the carbon footprint of training and operation phases are currently missing.

## Citation
```bibtex
@article{overlan2025forestcast,
  title={ForestCast: Forecasting Deforestation Risk at Scale with Deep Learning},
  author={Overlan, M. and Stanton, C. and Neumann, M. and others},
  year={2025}
}
```