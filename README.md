# Earthquake Early Warning System Using Machine Learning

## Project Overview

The Earthquake Early Warning System is a machine learning-based project designed to analyse seismic data and classify seismic events. It uses historical earthquake data and machine learning algorithms to distinguish between earthquake-related events and explosions.

The system combines data preprocessing, model training, performance evaluation and a Flask-based web interface to make seismic data analysis accessible through a browser.

## Objectives

- Analyse seismic parameters and identify patterns in historical seismic data.
- Classify seismic events using machine learning algorithms.
- Compare multiple classification models using performance metrics and confusion matrices.
- Provide an interactive interface for entering seismic information and viewing prediction results.
- Present event classification and impact-related information in an understandable format.

## Dataset

The project uses `Earthquake_Warning_Datasets.csv`, containing **8,851 records** with seismic attributes such as:

- Latitude and longitude
- Depth and magnitude
- Magnitude type
- Number of seismic stations
- Gap and minimum distance
- RMS (Root Mean Square)
- Seismic network information
- Horizontal error, depth error and magnitude error

The dataset contains two target categories:

- Earthquake warning – 2,177 records
- Explosion – 6,674 records

## Machine Learning Algorithms

Four classification algorithms are implemented and evaluated:

1. **K-Nearest Neighbors (KNN)** – Classifies events based on similarities between data points.
2. **Decision Tree** – Uses decision-based rules to classify seismic events.
3. **Support Vector Machine (SVM)** – Identifies decision boundaries between event categories.
4. **Random Forest** – Combines multiple decision trees for classification.

Model evaluation includes accuracy, precision, recall, F1-score and confusion matrices.

## System Workflow

1. Load the historical seismic dataset.
2. Preprocess the data and handle missing values.
3. Encode categorical features into numerical values.
4. Split the dataset into training and testing sets.
5. Train and evaluate the machine learning classifiers.
6. Accept seismic parameters through the web interface.
7. Display the predicted event category and relevant analysis results.

## Application Features

- Browser-based interface developed using Flask.
- Input form for seismic parameters.
- Earthquake and explosion classification.
- Comparison of machine learning model performance.
- Confusion matrix-based evaluation.
- Impact-level and estimated affected-area displays.

## Screenshots

### Input Interface

![Input Details](screenshots/Enter%20details1.jpg)

![Additional Input Details](screenshots/Enter%20details2.jpg)

### Seismic Analysis and Results

![Impact Level](screenshots/impact%20level.jpg)

![Estimated Earthquake Effects](screenshots/earthquzke%20effect.jpg)

### Model Performance

![Model Performance Comparison](screenshots/model%20performance%20comparision.jpg)

## Technologies Used

- **Python** – Core programming language
- **Pandas and NumPy** – Data processing and numerical operations
- **Scikit-learn** – Machine learning algorithms and evaluation
- **Matplotlib and Seaborn** – Data visualisation
- **Flask** – Web application framework
- **Jupyter Notebook** – Model development and experimentation
- **HTML and CSS** – User interface

## Running the Project

Clone the repository:

```bash
git clone https://github.com/Abhishek-2709/earthquake-early-warning-system.git
```

Navigate to the project directory:

```bash
cd earthquake-early-warning-system
```

Install the required libraries:

```bash
pip install pandas numpy scikit-learn seaborn matplotlib flask jupyter
```

Launch Jupyter Notebook:

```bash
jupyter notebook
```

Open `earthquake.ipynb` and execute the relevant cells to train the models and run the application.

## Research Direction

The accompanying research paper also explores the potential use of P-wave arrival times and differential arrival times between seismic stations for improving earthquake source-location estimation. This represents a research direction for enhancing the speed and accuracy of earthquake early warning systems.

## Project Team

- Gopalapuram Abhishek
- Gurram Satwik Reddy
- Neelawar Shiva Ashish

**Institution:** Sreenidhi Institute of Science and Technology, Hyderabad, India.

**Project Guide:** Mr. Veer Kumar

## Disclaimer

This project is an academic machine learning prototype for seismic-event classification and analysis. It is not a certified earthquake prediction or public warning system.
