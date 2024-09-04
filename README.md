# Titanic-Survival-Prediction-A-Journey-Through-the-Data

## Project Overview
This project aims to build a predictive model that determines which passengers were more likely to survive the Titanic disaster. Utilizing passenger data such as age, gender, socio-economic class, and family size, we explore various machine learning techniques to gain insights and improve prediction accuracy.

## Dataset
The dataset contains detailed information on 1,309 passengers aboard the Titanic. Key features include:
- **pclass**: Passenger class (1st, 2nd, 3rd)
- **survived**: Survival indicator (0 = No, 1 = Yes)
- **sex**: Gender of the passenger
- **age**: Age of the passenger
- **sibsp**: Number of siblings/spouses aboard
- **parch**: Number of parents/children aboard
- **fare**: Fare paid for the ticket
- **embarked**: Port of Embarkation (C = Cherbourg; Q = Queenstown; S = Southampton)
- **family_size**: Combined number of siblings/spouses and parents/children aboard

## Data Preprocessing
- **Handling Missing Values**: 
  - Filled missing values in `age` and `fare` with the median.
  - Filled missing values in `embarked` with the mode.
  - Dropped columns with a high percentage of missing values (`cabin`, `boat`, `body`, `home.dest`).

- **Categorical Variable Encoding**:
  - Converted `sex` to numeric (0 for male, 1 for female).
  - One-hot encoded `embarked`.

- **Feature Engineering**:
  - Created a new feature `family_size` by combining `sibsp` and `parch`.
  - Dropped unnecessary columns like `name` and `ticket`.

## Exploratory Data Analysis (EDA)
- Visualized the distribution of survival using count plots.
- Explored relationships between survival and other features like age, sex, and passenger class.

## Model Building
We experimented with several machine learning models to predict survival, including:
- **Logistic Regression**
- **Random Forest Classifier**
- **Support Vector Machine (SVM)**
- **K-Nearest Neighbors (KNN)**
- **Gradient Boosting Classifier**
- **AdaBoost Classifier**

## Model Evaluation
We used the following metrics to evaluate model performance:
- **Accuracy Score**
- **F1 Score**
- **Confusion Matrix**
- **Classification Report**

## Results
The Random Forest Classifier and Gradient Boosting Classifier yielded the best performance, with high accuracy and balanced F1 scores. Further hyperparameter tuning was performed using GridSearchCV to optimize the models.

## Conclusion
This project demonstrates the process of building a binary classification model to predict Titanic survival. Through data preprocessing, EDA, and model experimentation, we gained insights into the key factors influencing passenger survival and successfully developed a predictive model.

## How to Run
1. Clone the repository:
    ```bash
    git clone https://github.com/your-username/Titanic-Survival-Prediction.git
    ```
2. Install the required dependencies:
    ```bash
    pip install -r requirements.txt
    ```
3. Run the Jupyter notebook to explore the analysis and model building process.

## Future Enhancements
- Explore additional feature engineering techniques.
- Experiment with ensemble methods for model improvement.
- Perform a deep learning approach to further enhance predictions.

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

By **Sama Amr Habib**
