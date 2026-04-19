### **Automated Predictive Modeling of COVID-19 Fatality Outcomes Using Dataiku AutoML**
<img width="1280" height="409" alt="Screen Shot 2026-04-19 at 19 39 11" src="https://github.com/user-attachments/assets/7e8480a7-7e15-4388-bda3-fad258164932" />

### **Project Overview**
This project involved the design and implementation of an end-to-end Machine Learning pipeline to address the critical need for high-accuracy fatality predictions during a global health crisis. By leveraging the no-code AutoML capabilities of the Dataiku DSS platform, I developed a model utilizing global COVID-19 epidemiological data. The final predictive model achieved an accuracy exceeding 90%, providing a robust tool for identifying regions at high risk for increased mortality.

### **Business Understanding**
The primary stakeholders for this analysis include public health administrators, government policy makers, and emergency response coordinators. The core business problem was the rapid and accurate identification of geographic hotspots where fatality rates might surge, which is essential for the proactive allocation of limited medical resources, such as ventilators, PPE, and specialized personnel. Research indicates that data-driven resource distribution can significantly reduce strain on healthcare systems and improve patient outcomes during peak infection periods.

### **Data Understanding**
The analysis utilized a comprehensive dataset encompassing global COVID-19 metrics joined with regional mapping data.
* **Data Sources:** The primary dataset contained features such as confirmed cases, active cases, recoveries, and geographical coordinates. A secondary `Continent_Country_Mapping` dataset was integrated to provide macro-level regional context.
* **Timeframe:** The data reflects a critical global snapshot as of **February 5, 2021**.
* **Data Limitations:** The dataset is a snapshot in time; therefore, it does not account for subsequent viral mutations or the introduction of vaccination programs. Additionally, "Recovered" data in some regions may be underreported due to varying local reporting standards.
* **Exploratory Insights:** Initial analysis highlighted a significant correlation between the volume of active cases and subsequent fatalities, though the "Case Fatality Ratio" varied significantly by continent.

### **Modeling and Evaluation**
To maximize efficiency and model robustness, I engineered a no-code ML pipeline using **Dataiku AutoML**. This approach allowed for the rapid benchmarking of multiple algorithms to identify the optimal predictor for fatality outcomes.
* **Modeling Approach:** The pipeline automated feature engineering, handling missing values in geographical data, and selecting the best-performing algorithm (typically Random Forest or Gradient Boosting in similar AutoML configurations).
* **Evaluation Metrics:** The primary metric for success was **Classification Accuracy**. The model successfully surpassed the project benchmark, delivering a **predictive accuracy of over 90%**. This high level of precision ensures that the model can be used as a reliable decision-support tool.
<img width="537" height="318" alt="Screen Shot 2026-04-15 at 16 49 22" src="https://github.com/user-attachments/assets/45d8feed-8132-49cf-a002-ac4d59cd1b63" /> <img width="999" height="222" alt="Screen Shot 2026-04-19 at 18 52 15" src="https://github.com/user-attachments/assets/1ff92d5e-f3f6-4fbe-bd70-e39a52ac53ac" />

### **Conclusion**
The project demonstrates that high-performance machine learning solutions can be deployed rapidly without manual coding, provided there is a structured data pipeline. Based on the model results, I recommend that health organizations prioritize logistical support for regions where predicted fatality thresholds are breached, even if current confirmed counts appear stable.

**Future Steps:**
* I plan to incorporate time-series data into the pipeline to transition from snapshot predictions to dynamic trend forecasting.
* Integrating demographic data (such as median age or healthcare infrastructure indices) could further refine the model's sensitivity to regional variations in fatality rates.<img 
