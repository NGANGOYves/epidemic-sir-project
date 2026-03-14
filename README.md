# Epidemic Modeling Using SIR Model

This project demonstrates the spread of an epidemic using the **SIR (Susceptible-Infected-Recovered) model** based on real-world COVID-19 data from Kaggle. It is a Python-based project using Jupyter Notebook to analyze, simulate, and visualize epidemic dynamics.

---

## Project Overview

**Objective:**  
The goal of this project is to model the evolution of an epidemic in a country using real data. The SIR model predicts the number of susceptible, infected, and recovered individuals over time. This helps understand the dynamics of disease spread and estimate key epidemiological parameters.

**Dataset:**  
- Source: Kaggle COVID-19 dataset (`covid_19_data.csv`)  
- The code automatically selects the first country available in the dataset for analysis.  

**Model:**  
- Compartmental SIR model:  
  - **S(t):** Susceptible population  
  - **I(t):** Infected population  
  - **R(t):** Recovered population  
- Differential equations govern the flow:  

![Equation DF](results/figures/eqn.png)  

- **β (beta):** infection rate  
- **γ (gamma):** recovery rate  
- **R₀ = β / γ:** basic reproduction number  

**Outputs:**  
- Epidemic curves and logarithmic growth  
- SIR compartments (real vs. model simulation)  
- Tables of the first few days of SIR compartments  
- Estimated parameters (β, γ, R₀)

---

## Folder Structure


epidemic-sir-project/
data/ # Place your Kaggle dataset here
results/ # Generated figures will be saved here automatically
figures/
     sir_project.ipynb # Main Jupyter notebook with full code is at this level
     .gitignore # To exclude unnecessary files from git
     README.md #for more explanation find out this readme


---

## Usage Instructions

1. Place the Kaggle dataset CSV file (`covid_19_data.csv`) in the `data/` folder.  
2. Open `sir_project.ipynb` in **Jupyter Notebook**.  
3. Run all cells sequentially.  
4. Figures and graphs will automatically be saved in `results/figures/`.  
5. View the first few days of the SIR table directly in the notebook or use it in your report.  

---

## Main Features

- Automatically detects the country from the dataset.  
- Constructs **SIR compartments** for susceptible, infected, and recovered populations.  
- Fits the **SIR model to real data** using numerical simulation and optimization.  
- Estimates **β, γ, and R₀** parameters.  
- Produces **clear visualizations**:  
  - Epidemic curve (daily confirmed cases)  
  - Logarithmic growth  
  - Real SIR data  
  - Model vs real infected  
  - Full SIR simulation  
- Provides **tables of first few days** for reporting purposes.  

---

## Figures

### 1. Epidemic Curve
![Epidemic Curve](results/figures/epidemic_curve.png)  
*Daily confirmed cases from the dataset.*

### 2. Logarithmic Growth
![Log Growth](results/figures/log_growth.png)  
*Shows the exponential growth trend.*

### 3. Real SIR Data
![Real SIR](results/figures/sir_real_data.png)  
*Real Susceptible, Infected, and Recovered values.*

### 4. Model vs Real Data
![Model vs Real](results/figures/model_vs_real.png)  
*Comparison between SIR model prediction and real infected cases.*

### 5. Full SIR Simulation
![SIR Simulation](results/figures/sir_simulation_fitted.png)  
*Simulated SIR compartments using fitted parameters.*

---

## Results

After running the notebook, the project outputs:

- **Estimated β (infection rate)**  
- **Estimated γ (recovery rate)**  
- **Basic reproduction number R₀**  
- **First 10 days of SIR table**  
- High-quality figures saved for reports or presentations  

These results can be directly used in your project report for visualization and discussion.

---

## License

This project is **for educational and research purposes only**.  

---

## Author

**Yves Lucas NGANGO**  
[GitHub Profile](https://github.com/NGANGOYves)

---

