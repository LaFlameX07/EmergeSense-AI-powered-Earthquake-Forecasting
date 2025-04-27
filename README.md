# 🌎 EmergeSense – AI-powered Earthquake and Flood Forecasting

![EmergeSense Banner]([https://user-images.githubusercontent.com/your_banner_link_here.png](https://media.istockphoto.com/id/2007470156/photo/seismic-waves-analysis.jpg?s=612x612&w=0&k=20&c=pFIxaMgK99GRzRFOHCijZgZ6ieGbQKywsywHMzIAmiw=)) <!-- (Optional: Add a banner image here) -->

## 📖 About the Project
**EmergeSense** is an AI-powered disaster response system that integrates **machine learning** and **geospatial data analysis** to **predict earthquakes and floods** in real-time.  
Our goal is to **enhance disaster preparedness** by providing early warnings and actionable insights to help mitigate the impact of natural disasters.

---

## 🚀 Key Features

- 🔥 **Earthquake Forecasting** using USGS Seismic Data.
- 🌊 **Flood Prediction** using NASA SRTM Elevation Contours and CHIRPS Rainfall Data.
- 🧠 **AI Models** built with XGBoost and Contour Analysis.
- 📡 **Real-time Disaster Monitoring** and Risk Assessment.
- 📍 **Impact Radius Estimation** for Earthquake Magnitudes.
- 🌐 **Fully Scalable** to other disasters like landslides, tsunamis, etc.

---

## 🔍 Earthquake Prediction Pipeline

1. **Seismic Data (USGS):**  
   - Predicts **earthquake probability** for the next 7 days.
   - Estimates **latitude, longitude**, and **depth**.

2. **Magnitude Prediction:**  
   - Using predicted depth and coordinates.
   - Calculates **magnitude** of the event.

3. **Impact Radius Calculation:**  
   - Applies empirical formula:  
     \[
     \text{Radius (in km)} = 10^{(-1.83 + 0.45 \times \text{Magnitude})}
     \]

4. **Output:**  
   - Forecast of upcoming earthquakes with location, magnitude, and impact radius.

---

## 🌊 Flood Prediction Pipeline

1. **Elevation Contour Analysis (NASA SRTM):**  
   - Identifies **low-lying flood-prone areas**.

2. **Rainfall Contour Analysis (CHIRPS Data):**  
   - Detects regions experiencing **high precipitation**.

3. **Overlay Mapping:**  
   - Overlapping zones of low elevation and high rainfall predict **high-risk flood zones**.

4. **Output:**  
   - **Flood susceptibility maps** showing potential risk areas.

---

## 🛠️ Tech Stack

| Technology | Purpose |
|:----------|:--------|
| Python | Core Programming |
| XGBoost | Earthquake Prediction |
| Pandas & NumPy | Data Preprocessing |
| h5py / Pickle | Model Saving and Loading |
| Scikit-learn | Regression Analysis |
| Matplotlib & Seaborn | Data Visualization |
| NASA SRTM, CHIRPS, USGS | Data Sources |

---

## 🗂️ Folder Structure

📦EmergeSense ┣ 📜 New_Amit_Earthquake_Forecasting.ipynb ┣ 📜 cleaned_earthquake_data.csv ┣ 📜 multimodal_model.pkl ┣ 📜 README.md ┗ 📂 (Data Sources Folder)

---

## 📈 Results

| Task | Accuracy / Insight |
|:----|:------------------|
| Earthquake occurrence prediction | Achieved high forecasting reliability using seismic data. |
| Magnitude prediction | Empirical radius correlation successfully implemented. |
| Flood-prone area identification | Accurate contour-based flood risk mapping. |

---

## 🌟 Unique Selling Proposition (USP)

- **Multi-modal disaster forecasting**: Combines structured seismic data and geospatial contour data.
- **Real-time, scalable, and actionable**: Designed for immediate deployment and future extensibility.
- **Empowers disaster response teams** with predictive insights, not just alerts.

---

## ✨ Future Enhancements

- 🌪️ Expand to predict **cyclones and landslides**.
- 📱 Develop a **mobile app** for real-time public alerts.
- 📊 Integrate with **local government databases** for action planning.

---

## 🤝 Contributing

We welcome contributions!  
Please fork the repository and submit a pull request. 💻

---

## 📄 License

This project is open-source under the [MIT License](LICENSE).

---

## 🙌 Acknowledgements

- [USGS Earthquake Data API](https://earthquake.usgs.gov/)
- [NASA SRTM Elevation Data](https://www2.jpl.nasa.gov/srtm/)
- [CHIRPS Rainfall Data](https://www.chc.ucsb.edu/data/chirps)

---

# 🚀 Let's make disaster response faster, smarter, and better!
