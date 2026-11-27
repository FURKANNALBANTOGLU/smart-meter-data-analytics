# Smart Meter Data Analytics & Signal Processing

This repository contains a Python-based data analytics and digital signal processing (DSP) study on residential smart meter active power consumption data. The project focuses on extracting daily usage habits, identifying appliance operating modes, and analyzing periodic load patterns in both time and frequency domains.

## Key Analyses & Features
* **Time-Series Exploration:** Visualizes raw high-resolution (1-second) active power consumption (`Active Power (W)`) to track load fluctuations and peak demand periods.
* **Distribution & Operating Mode Detection:** Uses linear and logarithmic histograms paired with `scipy.signal.find_peaks` to isolate recurring power levels and distinct appliance/standby operating states.
* **Frequency-Domain Analysis (FFT & Spectrogram):** Removes the DC offset to compute single-sided Fast Fourier Transform (FFT) spectra and dB-scaled spectrograms, revealing periodic switching cycles and harmonic load behavior.
* **Daily Consumption Heatmaps:** Maps multi-day 24-hour consumption profiles (`00:00 – 24:00`) and applies a square-root transformation ($\sqrt{W}$) to enhance visual contrast between low-power standby periods and high-power peaks.

## Technologies Used
* **Language:** Python 3
* **Libraries:** NumPy, Pandas, SciPy (`fft`, `signal`), Matplotlib, Seaborn
* **Environment:** Google Colab

## Repository Structure
* `smart_meter_analysis.ipynb` – Complete Jupyter/Colab notebook containing data cleaning, signal processing algorithms, and visualizations.

## How to Run
1. Open `smart_meter_analysis.ipynb` directly in **Google Colab** or **Jupyter Notebook**.
2. Ensure standard scientific Python libraries (`numpy`, `pandas`, `scipy`, `matplotlib`, `seaborn`) are installed.
3. Run the cells sequentially to reproduce all time-domain, frequency-domain, and heatmap visualizations.

## Author
**Furkan Nalbantoğlu**  
Electrical & Electronics Engineering Student  
[GitHub Profile](https://github.com/FURKANNALBANTOGLU)
