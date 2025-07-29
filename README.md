# Finance Data Exploratory Analysis
This project demonstrates basic exploratory data analysis (EDA) on a financial survey CSV. It walks through:

1. Listing all files in `/kaggle/input`  
2. Loading the `Finance_data.csv`  
3. Dropping redundant numeric investment columns  
4. Plotting demographics and investment behavior with Seaborn & Matplotlib  

---

## 📁 File Structure

```

.
├── Finance\_data.csv        # Survey with demographics & investment variables
├── EDA\_notebook.ipynb      # Jupyter/Colab notebook containing the code below
└── README.md               # This file

````

---

## ⚙️ Requirements

```bash
pip install numpy pandas seaborn matplotlib tqdm torch torchvision albumentations opencv-python pillow
````

> All imports appear at the top of the notebook:
> `numpy, pandas, os, seaborn, matplotlib.pyplot, cv2, tqdm, torch, torchvision, albumentations`

---

## Usage

1. **Open in Kaggle or Colab**
   Copy the notebook into your environment, ensuring `Finance_data.csv` sits under `/kaggle/input/finance-data/Finance_data.csv`.

2. **Run all cells**

   * Lists input files
   * Reads the CSV into a DataFrame
   * Displays the first 5 rows
   * Drops the seven numeric columns:

     * `Mutual_Funds, Equity_Market, Debentures, Government_Bonds, Fixed_Deposits, PPF, Gold`
   * Creates plots:

     * **Gender** count
     * **Age** distribution
     * **Investment Avenue** and **Stock Market** by gender
     * **Factor** counts and by gender
     * **Purpose vs Age** point plot
     * **Duration** and **Invest\_Monitor** by gender

3. **Inspect outputs**
   Each plot appears inline; customize styling or add more charts as needed.


## 📊 Visualizations

* **Countplots** for categorical columns (`gender`, `age`, `Investment_Avenues`, `Stock_Marktet`, `Factor`, `Duration`, `Invest_Monitor`).
* **Pointplot** of `Purpose` vs. `age` to reveal trends across survey purposes.
