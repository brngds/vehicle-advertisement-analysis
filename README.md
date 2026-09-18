# 🚗 Vehicle Advertisement Analysis

Interactive web application for exploratory analysis of vehicle advertisements using **Python**, **Pandas**, **Plotly Express**, and **Streamlit**, with a focus on vehicle mileage distribution and the relationship between mileage and price.

## 📌 Context

Interactive data applications make exploratory analysis more accessible by allowing users to interact directly with visualizations instead of relying only on static reports or notebooks.

In this project, a vehicle advertisement dataset was explored and used to develop an interactive **Streamlit web application**. The application allows users to visualize vehicle mileage distribution and investigate the relationship between mileage and advertised price.

The project was developed as part of my Data Science studies and reorganized for portfolio presentation, combining exploratory data analysis, interactive visualization, software development, and cloud deployment.

## 🎯 Problem

The main objective was to transform a vehicle advertisement dataset into an accessible interactive analytical application.

The project addresses questions such as:

- How is vehicle mileage distributed across advertisements?
- How do advertised prices vary across different mileage levels?
- Can exploratory visualizations be made available through a simple interactive interface?
- How can a Python data application be deployed and made accessible online?

Beyond the analytical component, the project also demonstrates the process of building and deploying a functional data application.

## 📊 Dataset

The analysis uses `vehicles.csv`, containing **51,525 vehicle advertisements and 13 variables**.

The available features include:

- `price` — advertised vehicle price
- `model_year` — vehicle model year
- `model` — vehicle model
- `condition` — vehicle condition
- `cylinders` — number of cylinders
- `fuel` — fuel type
- `odometer` — vehicle mileage
- `transmission` — transmission type
- `type` — vehicle type
- `paint_color` — vehicle color
- `is_4wd` — four-wheel-drive indicator
- `date_posted` — advertisement publication date
- `days_listed` — number of days the advertisement remained listed

## 🔎 Approach

The project followed a workflow combining exploratory analysis and application development:

1. Data loading and initial inspection
2. Dataset structure and data type validation
3. Missing value analysis
4. Duplicate record verification
5. Exploration of vehicle mileage distribution
6. Analysis of the relationship between mileage and price
7. Development of interactive visualizations with Plotly Express
8. Integration of visualizations into a Streamlit application
9. Configuration of the application environment
10. Deployment of the web application

## 🧹 Data Quality

The dataset was inspected before visualization to understand its structure and potential quality issues.

The analysis identified missing values in:

- `model_year`
- `cylinders`
- `odometer`
- `paint_color`
- `is_4wd`

No fully duplicated rows were identified.

Because the objective of this project is lightweight exploratory visualization and application development, missing values were documented rather than artificially replaced solely for the purpose of generating the visualizations.

## 📈 Exploratory Analysis

### Vehicle mileage distribution

A histogram was created to explore the distribution of `odometer` values across vehicle advertisements.

The visualization provides an overview of the mileage profile of vehicles available in the dataset and helps identify how advertisements are distributed across different mileage ranges.

### Price vs. mileage

A scatter plot was created to investigate the relationship between:

- vehicle mileage (`odometer`);
- advertised price (`price`).

The visualization shows substantial price variation among vehicles with similar mileage levels, indicating that mileage alone does not explain differences in advertised prices.

Other characteristics such as model, model year, condition, and vehicle type may also contribute to pricing differences.

## 🖥️ Streamlit Application

The exploratory visualizations were incorporated into an interactive web application developed with **Streamlit**.

Users can choose whether to display:

- a histogram of vehicle mileage;
- a scatter plot comparing vehicle mileage and price.

The charts are generated with **Plotly Express**, providing interactive visualization directly in the browser.

## 🌐 Live Application

The application is deployed and publicly accessible through Render:

**[Open the Vehicle Advertisement Analysis App](https://new-q9zv.onrender.com)**

> The application is hosted on Render and may take a few moments to start if the service is inactive.

## 💡 Key Findings

The exploratory analysis highlights several characteristics of the available vehicle advertisement data:

- vehicle advertisements cover a wide range of mileage values;
- mileage distribution is concentrated in lower and intermediate ranges, with fewer observations at very high mileage levels;
- advertised prices vary substantially even among vehicles with similar mileage;
- mileage alone is therefore insufficient to explain vehicle pricing;
- interactive visualizations make it easier to explore these patterns directly through the web application.

These observations describe patterns in the available dataset and should not be interpreted as causal relationships.

## 🚀 Project Applications

This project demonstrates how exploratory data analysis can be transformed into an accessible analytical product.

The same workflow can be applied to:

- interactive business dashboards;
- marketplace inventory analysis;
- product and pricing exploration;
- self-service analytical tools;
- rapid analytical prototypes;
- deployment of Python-based data applications.

## ⚠️ Limitations

This project focuses on exploratory visualization and web application development rather than comprehensive vehicle price modeling.

Missing values were not imputed, and the analysis does not control for all characteristics that may influence vehicle prices.

Therefore, the observed relationship between mileage and price should be interpreted descriptively rather than as evidence of causality.

## 🛠️ Technologies

- Python
- Pandas
- Plotly Express
- Streamlit
- Jupyter Notebook
- Render
- Git
- GitHub

## 📁 Repository Structure

vehicle-advertisement-analysis/
│
├── README.md
├── app.py
├── vehicles.csv
├── requirements.txt
├── .gitignore
│
├── .streamlit/
│   └── config.toml
│
└── notebooks/
    └── EDA.ipynb

## ▶️ Running the Application Locally

Clone the repository, install the required dependencies, and start the Streamlit application:

```bash
pip install -r requirements.txt
streamlit run app.py
