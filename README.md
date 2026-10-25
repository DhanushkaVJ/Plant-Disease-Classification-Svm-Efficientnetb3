# Plant Disease Classification Using SVM and EfficientNetB3

A machine learning project exploring automated plant disease classification using leaf images from the PlantVillage dataset. This project implements and evaluates a traditional Support Vector Machine (SVM) baseline and an EfficientNetB3 transfer-learning model.

## Project Highlights

- Classified 38 plant disease and healthy-leaf categories.
- Extracted handcrafted texture and colour features using Local Binary Patterns (LBP) and RGB histograms.
- Optimised the SVM using GridSearchCV with 3-fold cross-validation.
- Applied transfer learning and fine-tuning with EfficientNetB3.
- Evaluated model performance using accuracy metrics, classification reports, and confusion matrices.

## Results

| Model | Evaluation metric | Accuracy |
|---|---|---:|
| SVM | Training accuracy | 98.49% |
| SVM | Validation accuracy | 90.85% |
| SVM | Test accuracy | 90.58% |
| EfficientNetB3 | Validation accuracy | 91.26% |

**Note:** The reported validation and test accuracies come from different evaluation sets and should not be interpreted as a direct comparison on identical data.

## Technologies

Python · Scikit-learn · TensorFlow · Keras · OpenCV · Scikit-image · NumPy · Pandas · Matplotlib · Seaborn · Jupyter Notebook

## Dataset

PlantVillage dataset: [GitHub repository](https://github.com/spMohanty/PlantVillage-Dataset)

The dataset contains 54,305 images across 38 classes. The dataset itself is not included in this repository.

## Repository Contents

- `SVM.ipynb` — handcrafted feature extraction, SVM training, hyperparameter optimisation, and evaluation.
- `EfficientNetB3.ipynb` — transfer learning, fine-tuning, and model evaluation.
- `requirements.txt` — Python package dependencies.

## How to Run

1. Clone or download this repository.
2. Obtain the PlantVillage dataset from the source above.
3. Install dependencies using `pip install -r requirements.txt`.
4. Update the dataset paths in each notebook.
5. Run the notebooks from top to bottom in Jupyter Notebook or a compatible environment.

## Limitations and Future Work

The PlantVillage dataset contains images captured under controlled conditions. Further testing on real-world field images is needed to assess robustness under changing lighting, backgrounds, and leaf orientations. Future work could also investigate lightweight deployment and evaluation on a shared, independent test set.

## Authors

- Dhanushka Jayasinghe
- Mridul Raj Poudel

Master of Applied Technologies – Computing, Unitec Institute of Technology.
