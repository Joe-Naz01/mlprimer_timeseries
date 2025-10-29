# ML Primer (Notebook)

A hands-on primer that walks through:
- Plotting two time series from CSVs
- **Classification:** SVM on the Iris dataset
- **Regression:** Linear model on California Housing
- **Audio:** Inspecting heartbeat WAV files with `librosa`
- **Finance:** Multi-series stock price plot from `prices.csv`

## Contents (by section)
1) **Time series without time axis**
   - Reads `data.csv` and `data2.csv`
   - Plots first 1000 points from each

2) **Iris classification with SVM**
   - Uses `LinearSVC` and an `SVC` pipeline with `StandardScaler`
   - 2D feature slice for visualisation (petal length/width)

3) **California Housing regression**
   - Fetches dataset via `sklearn.datasets.fetch_california_housing`
   - Fits linear regression (`sklearn.linear_model`)
   - Predicts over a 1-D input grid and overlays regression line

4) **Audio inspection (heartbeat)**
   - Loads `*.wav` files with `librosa`
   - Visualises waveform over time

5) **Prices dataset (multi-company)**
   - Reads `prices.csv`
   - Converts index to datetime
   - Plots multiple columns as price series

## Getting Started
```bash
#git clone
git clone https://github.com/Joe-Naz01/mlprimer_timeseries.git
cd mlprimer_timeseries
# (Recommended) create a virtual environment
python -m venv .venv
# Windows
.venv\Scripts\activate
# macOS/Linux
source .venv/bin/activate

pip install -r requirements.txt
