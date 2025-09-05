
# Parkinson’s Detection Using Quantum Machine Learning


Parkinson’s disease (PD) is a neurological disorder that affects movement and speech, causing symptoms such as tremors, stiffness, and slow motion. Early detection is crucial for managing the disease and improving quality of life.

This project leverages Quantum Machine Learning (QML) techniques, such as Quantum SVMs (QSVM), to predict Parkinson’s disease from patient data. QML can efficiently process complex, high-dimensional features, potentially improving accuracy compared to classical approaches. 


# Data
- we recieved a 750 X 756 dataset apporximated taht features multiple brain readings that could help recognise parkinsons.

- we first scaled the data to better be inline.
- we used principle component analysis (PCA) to decrease the number of features in the dataset.
- we then encoded about 64 pcas which we chose via trial and error to match the number of qubits chosen which was 6.


# Classical approach 
- we first developed multiple models for testing including SVM ,Neural Networks , CatBoost , and XGBoost. they all preformed similarly except catboost and xgboost preformed noticeably better providing an accuracy of 92 why the others provided an accruacy of around 86.


# Quantum approach
we developed a QSVM due to its counterparts preformance in the classical approach, and we also dont have access to many Quantum models due to the fact that its a new field (QML).


#Repository Structure 
```text
.
└─ parkinsons/
    ├─ catboost_info/
    │   ├─ learn/
    │   ├─ catboost_training.json
    │   ├─ learn_error.tsv
    │   └─ time_left.tsv
    ├─ parkinsons.data
    ├─ pd_speech_features.csv
    ├─ qsvm_training.ipynb
    ├─ quantum_kernel.npy
    ├─ test.ipynb
    ├─ test_data.npy
    ├─ test_hardware.ipynb
    ├─ classical_model_testing_main.ipynb
    └─ train_data.npy

```
# contribution

this project was made in collaboration with Nasser al Bess , Kinda Mashal, Khaled Abu Qutish, Nour Abu Ghazaleh , Rama Husseen , and Yousef Rihani.
it was made for the Bibliotheca Alexandria Quantum Hackathon 2025.





