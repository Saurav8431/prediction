🌾 AI-Powered Agricultural Parcel Profitability Analysis

This project provides an AI-driven system to evaluate the profitability of agricultural land parcels using a GeoJSON polygon. It integrates Google Earth Engine datasets and a trained machine-learning model to estimate crop suitability and investment returns.

🚀 Features

Paste or upload GeoJSON parcel polygons

Automatic extraction of:

NDVI, NDWI (Vegetation & Water Indices)

DEM & Slope

Rainfall, Temperature, Wind

Historical Water Occurrence

Soil Texture (Sand Content)

AI-based 3-Class Profitability Classification

Visual Profitability Map (Low / Medium / High)

Automatic parcel area calculation (ha)

Investment-based ROI Estimation (INR)

Powered by Google Earth Engine + Random Forest model

📊 Example Output

Parcel Profitability Summary:

Average Predicted Profitability: 48.98%

Estimated Return on Investment: ₹31,856.69

Parcel Area: 0.64 hectares

The profitability map displays:

Red → Low profit zones

Yellow → Medium

Green → High

🛰 NASA & ESA Satellite Data (Updated)

This project uses multi-satellite, multi-agency Earth observation datasets, primarily accessed through Google Earth Engine, ensuring regularly updated and scientifically reliable data for agricultural analysis.

🌍 NASA Missions

NASA SRTM (Shuttle Radar Topography Mission) — Provides 30m global elevation data for DEM and slope calculations.

NASA GLDAS / POWER (Optional in extended version) — Climate and radiation datasets used for enhanced environmental modeling.

🛰 ESA Missions (European Space Agency)

Sentinel‑2 MSI — High‑resolution 10m multispectral imagery used to derive:

NDVI (vegetation health)

NDWI (water index)

Soil/vegetation pattern detection

🌦 Climate & Weather

ECMWF ERA5‑Land — Global climate reanalysis providing daily temperature, rainfall, and wind speed.

🌊 Hydrology

JRC Global Surface Water — 36‑year global archive used to compute long‑term water occurrence and flood risk.

🌱 Soil

SoilGrids (ISRIC) — Updated soil texture datasets including sand content, ideal for assessing soil suitability.

This combined dataset ensures a high‑accuracy, multi‑year, multi‑sensor agricultural profitability assessment.



🧠 Machine Learning

Model: Random Forest Classifier

Trained on expert-labeled agricultural profitability datasets

Predicts profitability class using multi-year satellite-derived features

🛠 How to Use

Draw or paste your parcel GeoJSON polygon

Enter your investment amount (INR)

Click Submit

View:

Profitability map

Return on investment

Parcel area

Summary statistics

📁 Project Structure

├── app.py                # Gradio / backend logic
├── model.pkl             # Trained Random Forest model
├── utils/                # Helper scripts
│   ├── ee_features.py    # Earth Engine feature extraction
│   └── preprocessing.py  # Cleaning / transformations
├── assets/               # Images & icons
└── README.md             # Documentation

🤝 Contributions

Contributions, bug reports, and suggestions are welcome! Feel free to open an issue or submit a pull request.

📬 Contact

Author: Saurav KumarEmail: sauravt735@gmail.com

⭐ Support

If you found this project useful, please star the repository on GitHu
