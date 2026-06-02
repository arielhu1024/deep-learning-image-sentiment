# Notebooks

This directory contains the notebooks used for image sentiment classification and social media engagement analysis.

| Notebook | Purpose |
|---|---|
| `01_data_preprocessing.ipynb` | Loads the image dataset, creates train/validation/test splits, applies augmentation and normalization, and prepares DataLoaders. |
| `02_alexnet_binary_classification.ipynb` | Trains the AlexNet binary sentiment classifier for positive vs. negative images. |
| `03_resnet50_binary_classification.ipynb` | Trains the ResNet50 binary sentiment classifier and compares performance with AlexNet. |
| `04_alexnet_multiclass_classification.ipynb` | Trains AlexNet for four-class sentiment classification: happiness, anger, sadness, and melancholy. |
| `05_resnet50_multiclass_classification.ipynb` | Trains ResNet50 for four-class sentiment classification. |
| `06_engagement_analysis.ipynb` | Applies the best-performing binary sentiment model to Instagram brand posts and analyzes engagement outcomes. |

## Suggested Execution Order

1. Run `01_data_preprocessing.ipynb` to understand dataset preparation.
2. Run binary classification notebooks: `02` and `03`.
3. Run multi-class classification notebooks: `04` and `05`.
4. Run `06_engagement_analysis.ipynb` after the AlexNet binary model has been trained and saved.

## Notes

- The original notebooks were developed in Google Colab.
- File paths should be updated before running locally or in a new Colab environment.
- The dataset is not redistributed in this repository; see `data/README.md` for data availability details.
