#Developer Role Classification from Commit Messages

This project aims to predict the developer role (e.g., frontend, backend, fullstack, QA) based on commit records. It demonstrates a machine learning pipeline that includes data preprocessing, exploratory data analysis, traditional ML  modeling, and fine-tuning a Large Language Model (LLM) for this classification task.

The project emphasizes reproducibility, transparent decision-making, and a thorough evaluation of different modeling approaches.

## Project Structure

The repository contains the following artifacts:

- `preprocessing.ipynb`: A Jupyter notebook detailing the steps for loading, validating, and engineering features from the raw commit data.
- `EDA.ipynb`: A Jupyter notebook containing exploratory data analysis, including visualizations and observations about the dataset's characteristics.
- `modeling.ipynb`: A Jupyter notebook showcasing the training and evaluation of traditional ML models (Logistic Regression, Random Forest, XGBoost) and the fine-tuning and evaluation of a BERT-based LLM.
- `evaluation_report.pdf`: A PDF document summarizing the final model performance on the test set, analyzing major failure modes, and outlining lessons learned.
- `reflection.md`: A markdown file containing a short reflection on key design decisions made throughout the project.
- `annotated_examples.md`: A markdown file providing ten annotated examples of commit messages from different developer roles with explanations for their label assignments.
- `README.md`: This file, providing an overview of the project and instructions for reproduction.
- `final_dataset.csv`: The dataset used for this project.

## How to Reproduce Results

To reproduce the results presented in this project, follow these steps:

1.  **Clone the Repository:**
# Using venv
    python -m venv venv
    source venv/bin/activate # On Windows use `venv\Scripts\activate`

       jupyter notebook preprocessing.ipynb
        # Or run using command line tools like nbconvert if you prefer
        # jupyter nbconvert --to notebook --execute preprocessing.ipynb --inplace

           jupyter notebook EDA.ipynb
        # Or run using command line tools
        # jupyter nbconvert --to notebook --execute EDA.ipynb --inplace

          jupyter notebook modeling.ipynb
        # Or run using command line tools
        # jupyter nbconvert --to notebook --execute modeling.ipynb --inplace

