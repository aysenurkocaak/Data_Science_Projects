# Artificial Intelligence Mobile Banking Project

This project processes user-entered messages and predicts their category using a machine learning model. Below is a summary of how the process works and what each step does:

1. **Data Preparation:**
   - The dataset `banka.csv` is loaded, which contains labeled queries and corresponding categories.
   - The dataset is filtered to focus only on the `sorgu` (query) and `label` (category) columns.

2. **Preprocessing:**
   - A list of Turkish stopwords (commonly used words that have little meaning) is used to remove stopwords from the user-entered query.

3. **User Input:**
   - The user is prompted to enter a query (such as a message), and this query is added to the existing dataset.

4. **Feature Extraction:**
   - `CountVectorizer` is used to convert the text data in the `sorgu` column into numerical features, selecting the top 50 most important terms.

5. **Model Training:**
   - The dataset is split into training and test sets, with 70% of the data used for training and 30% used for testing.
   - A Random Forest Classifier model is trained using the training set.

6. **Prediction and Evaluation:**
   - The trained model predicts the category of the newly entered message.
   - The model's accuracy score is calculated using the test set to evaluate its performance.

7. **Results:**
   - The predicted category and accuracy score of the model are displayed to the user.

This process ensures that new queries entered into the system are classified into the correct categories using the trained model. This functionality is an important part of an automatic message classification system.

# Screenshots 📷

<p align="center">
  <img src="https://github.com/aysenurkocaak/Data_Science_Projects/blob/main/Ekran%20Görüntüsü%20(448).png" width="850"><br><br>
  <img src="https://github.com/aysenurkocaak/Data_Science_Projects/blob/main/Ekran%20Görüntüsü%20(447).png" width="850"><br><br>
  <img src="https://github.com/aysenurkocaak/Data_Science_Projects/blob/main/Ekran%20Görüntüsü%20(446).png" width="850">
</p>
