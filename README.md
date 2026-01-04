# SpaceX Falcon 9 First Stage Landing Prediction

A comprehensive data science project that predicts whether the Falcon 9 first stage will land successfully. This prediction is crucial for determining launch costs, as SpaceX advertises Falcon 9 rocket launches at $62 million compared to other providers costing upward of $165 million - with savings primarily due to first stage reusability.

<img width="1917" height="896" alt="dash_completed" src="https://github.com/user-attachments/assets/901e45fe-1d7c-47c0-beaa-03d352556d8b" />

## 📋 Project Overview

This project analyzes SpaceX launch data to predict first-stage landing success using machine learning techniques. The analysis covers data collection, wrangling, exploratory data analysis, visualization, and predictive modeling.

## 🚀 Features

- **Data Collection**: Gather SpaceX launch data via API and web scraping
- **Data Wrangling**: Clean and preprocess launch data for analysis
- **SQL Analysis**: Query and analyze launch data using SQL
- **Exploratory Data Analysis**: Statistical analysis and visualization of launch patterns
- **Geospatial Analysis**: Interactive maps showing launch site locations and success rates
- **Interactive Dashboard**: Real-time visualization dashboard built with Plotly Dash
- **Machine Learning**: Predict landing success using multiple classification algorithms

## 🛠️ Technologies Used

### Data Science & Analysis
- **Python 3.x**
- **Pandas** - Data manipulation and analysis
- **NumPy** - Numerical computing
- **SQLite** - Database queries and analysis

### Visualization
- **Matplotlib** - Static plotting
- **Seaborn** - Statistical visualization
- **Plotly** - Interactive visualizations
- **Folium** - Interactive maps

### Web Development
- **Dash** - Interactive web dashboard
- **BeautifulSoup4** - Web scraping
- **Requests** - HTTP requests

### Machine Learning
- **Scikit-learn** - ML algorithms and model evaluation
  - Logistic Regression
  - Support Vector Machines (SVM)
  - Decision Trees
  - K-Nearest Neighbors (KNN)

## 📊 Analysis Workflow

1. **Data Collection** (`jupyter-labs-spacex-data-collection-api.ipynb`)
   - Fetch launch data from SpaceX API
   - Extract relevant features (flight number, payload mass, orbit, launch site, etc.)

2. **Web Scraping** (`jupyter-labs-webscraping.ipynb`)
   - Scrape additional launch data from web sources
   - Complement API data with historical records

3. **Data Wrangling** (`labs-jupyter-spacex-Data wrangling.ipynb`)
   - Handle missing values
   - Feature engineering
   - Data type conversions
   - Create derived features

4. **SQL Analysis** (`jupyter-labs-eda-sql-coursera_sqllite.ipynb`)
   - Query launch database for insights
   - Aggregate statistics by launch site
   - Analyze success rates across different parameters

5. **Exploratory Data Analysis** (`edadataviz.ipynb`)
   - Statistical analysis of launch data
   - Visualization of trends and patterns
   - Correlation analysis between features

6. **Geospatial Analysis** (`lab_jupyter_launch_site_location.ipynb`)
   - Map launch site locations
   - Analyze proximity to coastlines, cities, and railways
   - Visualize success rates by location

7. **Machine Learning Prediction** (`SpaceX_Machine Learning Prediction_Part_5.ipynb`)
   - Train multiple classification models
   - Hyperparameter tuning
   - Model evaluation and comparison
   - Select best performing model

8. **Interactive Dashboard** (`spacex-dash-app.py`)
   - Real-time filtering by launch site
   - Success rate pie charts
   - Payload vs. success correlation scatter plots
   - Interactive payload range selection

## 🎯 Key Insights

- Launch site location significantly impacts landing success
- Payload mass correlates with landing success probability
- Certain booster versions have higher success rates
- Launch sites: CCAFS LC-40, VAFB SLC-4E, KSC LC-39A, CCAFS SLC-40

## 🚀 Getting Started

### Prerequisites

```bash
pip install pandas numpy matplotlib seaborn plotly dash scikit-learn requests beautifulsoup4 folium
```

### Running the Dashboard

```bash
python spacex-dash-app.py
```

The dashboard will be available at `http://127.0.0.1:8050/`

### Running Jupyter Notebooks

```bash
jupyter notebook
```

Then open any of the `.ipynb` files to explore the analysis.

## 📈 Dashboard Features

- **Launch Site Dropdown**: Filter data by specific launch sites or view all sites
- **Success Rate Pie Chart**: Visual representation of successful vs. failed landings
- **Payload Range Slider**: Filter launches by payload mass (0-10,000 kg)
- **Scatter Plot**: Correlation between payload mass and landing success, colored by booster version

## 🎓 Use Cases

- **Cost Estimation**: Predict launch costs based on landing success probability
- **Competitive Bidding**: Enable alternate companies to bid against SpaceX
- **Risk Assessment**: Evaluate launch success likelihood based on parameters
- **Strategic Planning**: Optimize launch configurations for higher success rates

## 📝 License

This project is for educational purposes.

## 🤝 Contributing

This is an educational project. Feel free to fork and extend the analysis.

## 📧 Contact

For questions or feedback about this project, please open an issue in the repository.

---

**Note**: This project uses historical SpaceX launch data and is intended for educational and analytical purposes only.
