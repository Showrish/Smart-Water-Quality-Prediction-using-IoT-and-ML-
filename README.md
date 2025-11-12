# Smart Water Quality Prediction for Aquaculture Using Machine Learning

This **capstone project** focuses on predicting water quality in aquaculture systems using machine learning. By analyzing parameters such as **pH**, **turbidity**, and **potability**, the system assists in monitoring and maintaining safe water conditions for aquatic life.

The project utilizes **LSTM**, **GRU**, and **CNN** models for predictive analysis and provides real-time insights through a web application built with **Streamlit** or **Flask**.  
It also integrates **Firebase** for live data updates and monitoring.  
Live web application: [https://waterquality-1dcdc.web.app/](https://waterquality-1dcdc.web.app/)

---

## Project Objectives

- Predict water potability and quality from real-time sensor data  
- Enable proactive management of aquaculture systems  
- Develop a modular and scalable machine learning pipeline  
- Provide real-time monitoring and visualization via Firebase  

---

## Technologies Used

- **Python 3.x**
- **TensorFlow / Keras**
- **scikit-learn**
- **Pandas**, **NumPy**
- **Streamlit** or **Flask**
- **Firebase (Realtime Database, Hosting)**
- **Matplotlib**, **Seaborn**
- **HTML / CSS / JavaScript** (for chatbot and frontend)

---

## Project Structure

```
smart-water-quality-prediction/
├── app.py                   # Main web application
├── code/                    # Code modules for data processing and modeling
│   ├── convert.py
│   ├── labelingdata.py
│   ├── ML.py
│   ├── model_architecture.json
│   ├── model_weights.weights.h5
│   └── scaler.pkl
├── data/                    # Dataset files
│   ├── augmented_water_data.xlsx
│   ├── water_data.xlsx
│   └── water_potability.xlsx
├── web/                     # Frontend chatbot files
│   └── fish_water_quality_chatbot.html
├── templates/               # HTML templates (if applicable)
├── requirements.txt         # Python dependencies
└── README.md                # Documentation
```

---

## How to Run the Project

### Step 1: Clone this repository
```bash
git clone https://github.com/YOUR_USERNAME/smart-water-quality-prediction.git
cd smart-water-quality-prediction
```

### Step 2: Install required packages
```bash
pip install -r requirements.txt
```

### Step 3: Run the application
For Flask:
```bash
python app.py
```

For Streamlit:
```bash
streamlit run app.py
```

---

## Example Dataset Columns

| Feature     | Description                    |
|-------------|--------------------------------|
| pH          | Acidity/alkalinity of water     |
| Turbidity   | Cloudiness / particle level     |
| Solids      | Total dissolved solids (ppm)    |
| Potability  | 1 = safe for drinking, 0 = unsafe |

---

## Key Features

- Predicts water potability using ML models (LSTM, GRU, CNN)  
- Visualizes trends in water quality data  
- Real-time monitoring using Firebase integration  
- Simple and clean web interface  
- Modular structure, easy to extend with additional sensors or models  
- Deployable on both cloud and local environments  

---

## Fish Water Quality Chatbot

The project includes a **Fish Water Quality Chatbot** built using **HTML, CSS, and JavaScript**.  
The chatbot integrates with the **Gemini API** to provide ideal water parameters for various fish species, including:

- Recommended pH range  
- Turbidity (NTU)  
- Total dissolved solids (mg/L)

**File:** `web/fish_water_quality_chatbot.html`

### How to Use
1. Open the HTML file in any browser.  
2. Enter the fish species name.  
3. Click **Get Water Conditions** to view the recommended parameters retrieved from the API.

---

## Example Use Cases

- Automated monitoring of aquaculture ponds  
- Early detection of unsuitable water conditions  
- Integration into IoT-based smart aquaculture systems  

---

## License

This project is licensed under the **MIT License**.  
You are free to use, modify, and distribute this project with appropriate attribution.

---

## Live Demo

**Web Application:** [https://waterquality-1dcdc.web.app/](https://waterquality-1dcdc.web.app/)
