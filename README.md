

# LSTM  - DonorsChoose Dataset

This project explores the use of Long Short-Term Memory (LSTM) networks to predict project approval on the DonorsChoose dataset. Different architectures are tested to optimize performance, combining LSTM layers with Convolutional Neural Networks (CNN) and embedding layers.

## Dataset
- **Dataset**: DonorsChoose project proposals dataset.
- **Features**: Text data (essays), categorical features (project categories, school states), and numerical data.
- **Target**: Project approval prediction.

## Models Implemented
1. **Model 1**:
   - Simple LSTM network with embedding layers for text input.
   - Used categorical and numerical features with dense layers.
   
2. **Model 2**:
   - LSTM network with TF-IDF filtering to remove low-information words.
   - Added hyperparameter tuning for embedding size, LSTM units, and dense layers.

3. **Model 3**:
   - Combined LSTM layers for text with 1D CNN layers for categorical features.
   - Tuned dropout and regularization to avoid overfitting.

## Key Results
- **Model 1**: Achieved AUC 0.74 on train data and 0.71 on test data.
- **Model 2**: Improved filtering of words helped achieve better results with AUC 0.77.
- **Model 3**: Best-performing model with AUC 0.76 on train data and 0.755 on test data.

## Conclusion
The combination of LSTM with CNN layers and careful hyperparameter tuning resulted in the best model performance, demonstrating that balancing text and categorical feature inputs can significantly improve predictive accuracy.

