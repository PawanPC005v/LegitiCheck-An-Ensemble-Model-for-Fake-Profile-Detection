# LegitiCheck-An-Ensemble-Model-for-Fake-Profile-Detection

This project is designed to classify users as either **genuine** or **fake** based on various features using machine learning. It includes a **User Legitimacy Interface** that allows users to manually input features and check the legitimacy of a user.

## Features
- **Data Preprocessing**: Handles non-numeric values, missing data, and feature scaling.
- **Deep Feature Extraction**: Utilizes a Multi-Layer Perceptron (MLP) to extract deep features from the dataset.
- **Classification**: Implements an XGBoost classifier for high-performance user classification.
- **User Legitimacy Interface**: Allows manual input of user features for classification.
- **Evaluation and Visualization**: Includes metrics like accuracy, confusion matrix, and ROC curve for model evaluation.

## Requirements
To run this project, ensure you have the following installed:
- Python 3.6 or higher
- Required Python libraries:
  - pandas
  - numpy
  - matplotlib
  - tensorflow
  - scikit-learn
  - xgboost
  - seaborn

You can install the required libraries using:
```bash
pip install -r requirements.txt
```

**Note**: Create a `requirements.txt` file with the following content:
```
pandas
numpy
matplotlib
tensorflow
scikit-learn
xgboost
seaborn
```

## Dataset
The project expects two CSV files:
1. `users.csv`: Contains data for genuine users.
2. `fusers.csv`: Contains data for fake users.

Place these files in the specified paths (`/content/users.csv` and `/content/fusers.csv`) or update the file paths in the script.

## How to Run
1. **Clone the Repository**:
   ```bash
   git clone https://github.com/your-repo/fake-user-classification.git
   cd fake-user-classification
   ```

2. **Prepare the Dataset**:
   - Ensure the `users.csv` and `fusers.csv` files are available in the appropriate paths.

3. **Run the Script**:
   Execute the Python script to train the model and launch the User Legitimacy Interface:
   ```bash
   python fake_user_classification_with_updated_interface.py
   ```

4. **Interact with the Interface**:
   - After training and evaluation, the script will launch an interactive interface.
   - Enter the required feature values:
     - `followers_count`
     - `friends_count`
     - `statuses_count`
     - `favourites_count`
     - `listed_count`
   - The script will classify the user as either **genuine** or **fake**, along with a probability score.

## Example Usage
Here is an example of how to use the interface:
```
--- User Legitimacy Interface ---
Enter the following feature values:

Enter value for followers_count: 500
Enter value for friends_count: 300
Enter value for statuses_count: 1000
Enter value for favourites_count: 50
Enter value for listed_count: 5

Prediction Results:
The user is likely GENUINE with a probability of 92.35%.
```

## Results
The script provides the following evaluation metrics:
- **Accuracy**: Measures the overall performance of the classifier.
- **Confusion Matrix**: Visualizes the classification performance.
- **ROC Curve**: Displays the trade-off between true positive and false positive rates.

## Project Structure
```
fake-user-classification/
│
├── fake_user_classification_with_updated_interface.py  # Main Python script
├── requirements.txt                                    # List of dependencies
├── users.csv                                           # Dataset for genuine users (example)
├── fusers.csv                                          # Dataset for fake users (example)
└── README.md                                           # Project documentation
```

## License
This project is licensed under the MIT License. Feel free to use and modify the code.

## Contributions
Contributions are welcome! If you encounter any issues or have ideas for improvements, feel free to open an issue or submit a pull request.

## Contact
For any queries, contact [PawanPC005v] at [https://www.linkedin.com/in/pawanmp05].
