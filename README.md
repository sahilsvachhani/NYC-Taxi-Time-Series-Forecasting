🚖 #NYC Taxi Time Series Forecasting

This project aims to forecast the demand for NYC taxi rides using time series analysis and machine learning techniques. By leveraging models like LightGBM and tools such as MLFlow, Streamlit, and Hopsworks, we aim to provide accurate predictions and deploy a functional machine learning pipeline with automated CI/CD workflows.


📌 ##Project Overview:

* Data Collection: Gathered historical NYC taxi ride data to analyze patterns and trends.
* Data Preprocessing: Cleaned and prepared the data for modeling, including handling missing values and feature engineering.
* Model Implementation: Utilized LightGBM for time series forecasting to predict ride demand.
* Hyperparameter Tuning: Employed MLFlow to track experiments and optimize model performance, achieving a Mean Absolute Error (MAE) below 6 rides.
* Automation: Set up GitHub Actions to automate feature engineering, model training, and inference pipelines.
* Deployment: Developed an interactive Streamlit application for real-time ride predictions and model monitoring.
* Data Management: Integrated with Hopsworks for efficient data storage, model tracking, and retrieval of time-series data.


🚀 ##Tech Stack

* Languages: Python
* Machine Learning: LightGBM, MLFlow
* Data Processing: Pandas, NumPy
* Visualization & Deployment: Streamlit, Matplotlib, Seaborn
* Automation & CI/CD: GitHub Actions
* Data Management: Hopsworks
* Version Control: Git, GitHub


📂 ##Project Structure:

📦 NYC-Taxi-Time-Series-Forecasting
│── .github/
│   └── workflows/          # GitHub Actions workflows
│── data/                   # Raw and processed data files
│── frontend/               # Streamlit application code
│── models/                 # Saved machine learning models
│── notebook/               # Jupyter notebooks for exploration and analysis
│── pipelines/              # Scripts for automated pipelines
│── src/                    # Source code for preprocessing, training, and inference
│── test/                   # Unit tests
│── requirements.txt        # Python dependencies
│── requirements_feature_pipeline.txt  # Dependencies for feature pipeline
│── requirements_with_version.txt      # Versioned dependencies
│── todo.md                 # Project to-do list
│── vscode_config.json      # VSCode configuration
│── README.md               # Project documentation


⚙️ ##Setup Instructions

###1. Clone the repository:

git clone https://github.com/sahilsvachhani/NYC-Taxi-Time-Series-Forecasting.git
cd NYC-Taxi-Time-Series-Forecasting

###2. Install dependencies:

pip install -r requirements.txt

###3. Run the Streamlit app:

streamlit run frontend/app.py


📈 ##Model Training & Hyperparameter Tuning

###1. Train the baseline model:

python src/train.py

###2. Perform hyperparameter tuning and log results in MLFlow:

python src/tune.py

###3. Track experiments in MLFlow UI:

mlflow ui


🌍 ##Deployment

* Automated Pipelines: GitHub Actions trigger feature engineering, training, and inference pipelines.
* Monitoring: Predictions and model performance are visualized using Streamlit.


📊 ##Results

* Achieved MAE < 6 rides after hyperparameter tuning.
* Successfully deployed a real-time forecasting app with Hopsworks integration.


🛠 ##Future Enhancements

* Implement additional time-series models such as Prophet, ARIMA, or FFT-based features for improved forecasting.
* Add location-based filtering to enhance prediction granularity.


🤝 ##Contributing

Contributions are welcome! Please fork this repository and submit a pull request if you have any improvements or suggestions.


📜 ##License

This project is licensed under the MIT License.