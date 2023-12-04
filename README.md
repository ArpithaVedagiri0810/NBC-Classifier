# NBC-Classifier
This Jupyter notebook contains code for training a Naive Bayes classifier on text data. The classifier is trained on a dataset and can be used to predict labels for new text data.

## Dependencies used

- Python 3
- Jupyter Notebook
- NumPy
- Pandas
- Scikit-learn

## Dataset

The code uses a dataset located at `/content/Generated_text.csv`. If you are running this code on your local system or a different environment, please make sure to update the dataset path accordingly.

## Code Explanation

1. Import necessary libraries.
2. Load the dataset.
3. Preprocess the data, including oversampling of a specific class.
4. Build a Naive Bayes classifier using Laplace smoothing.
5. Train the classifier on the training data.
6. Evaluate the classifier on a validation set to find the best alpha value.
7. Save the best classifier.

## How to Run

1. Open the provided Jupyter notebook (`NBC Ai.ipynb`).
2. Ensure that the required dependencies are installed.
3. Run each cell in the notebook sequentially.
4. The code will train the Naive Bayes classifier and print the accuracy for different alpha values.
5. The best classifier will be saved.
6. Test the classifier on new data from `test_essays.csv` and save the predictions in `submission.csv`.

## Output Files

- `submission.csv`: Contains the predictions for the test data.

## Note Regarding Dataset Path

The code uses a dataset located at `/content/Generated_text.csv`. If you are running this code on your local system or a different environment, please make sure to update the dataset path accordingly. You may need to change the path in the following line of code:

```python
# Update the dataset path with the location of the original dataset in your system
train = pd.read_csv('/content/Generated_text.csv')
