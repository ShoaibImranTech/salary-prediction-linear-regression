# Salary Prediction Using Linear Regression

This project uses Scikit-Learn's Linear Regression model to predict employee salaries based on experience, test scores, and interview scores.

## Dataset

The dataset (`hiring.csv`) contains the following features:
- **Experience** – Years of experience (may include text like "two", "five" which are converted to numbers)
- **Test Score** – Candidate's test score
- **Interview Score** – Candidate's interview score
- **Salary** – Target variable (salary in USD)

## Libraries Used

- `pandas` – Data loading and manipulation
- `numpy` – Numerical operations
- `scikit-learn` – Machine learning model (Linear Regression)
- `jupyter` – Interactive notebook environment

## Steps Performed

1. **Load Data** – Read `hiring.csv` using pandas
2. **Handle Missing Values** – Fill missing values in test scores and interview scores using the column mean
3. **Convert Experience Text to Numbers** – Transform word-form numbers (e.g., "two", "five") into integers using a word-to-number mapping
4. **Train Linear Regression Model** – Fit a `LinearRegression` model from scikit-learn on the processed data
5. **Make Predictions** – Predict salaries for new candidate profiles

## Example Usage

```python
# Predict salary for a candidate with:
# 2 years experience, test score 9, interview score 6
model.predict([[2, 9, 6]])
```

## How to Run

```bash
pip install -r requirements.txt
jupyter notebook salary_prediction.ipynb
```

## Project Structure

```
salary-prediction/
│
├── salary_prediction.ipynb   # Main notebook
├── hiring.csv                # Dataset
├── README.md                 # Project documentation
├── requirements.txt          # Dependencies
└── .gitignore                # Files to exclude from Git
```

## Upload to GitHub

```bash
git init
git add .
git commit -m "Initial commit"
git branch -M main
git remote add origin <your-repository-url>
git push -u origin main
```
