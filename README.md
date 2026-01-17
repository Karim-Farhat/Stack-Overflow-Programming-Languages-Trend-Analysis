# Stack Overflow Programming Languages Trend Analysis

This project analyzes the popularity of programming languages over time using Stack Overflow post data. The goal is to explore trends, compare languages, and visualize how interest in different technologies evolves.

The analysis is implemented in **Python** using **Pandas** for data manipulation and **Matplotlib** for visualization. The notebook was originally created in **Google Colab** and can be run locally with minimal setup.

---

## 📊 Dataset

The dataset (`QueryResults.csv`) contains Stack Overflow post counts grouped by date and programming language tag.

**Columns:**

* `DATE` – The date of the posts (monthly resolution)
* `TAG` – Programming language or technology tag (e.g., python, javascript)
* `POSTS` – Number of Stack Overflow posts for that tag on the given date

---

## 🛠️ Technologies Used

* Python 3
* Pandas
* Matplotlib
* Jupyter Notebook / Google Colab

---

## 📈 Analysis Workflow

1. **Load and Inspect Data**

   * Read the CSV file into a Pandas DataFrame
   * Inspect shape, counts, and basic statistics

2. **Data Cleaning & Preparation**

   * Convert `DATE` column to `datetime`
   * Pivot the table to get dates as rows and language tags as columns
   * Handle missing values by filling them with zeros

3. **Exploratory Data Analysis (EDA)**

   * Aggregate post counts by language
   * Analyze how frequently each language appears in the dataset

4. **Visualization**

   * Plot individual language trends (e.g., Python)
   * Compare multiple languages on the same plot
   * Plot all languages together for a global comparison

5. **Rolling Averages**

   * Apply a rolling window (10 periods) to smooth trends
   * Visualize long-term popularity trends more clearly

---

## 📉 Visualizations Included

* Python post count over time
* Python vs. Java / JavaScript comparison
* All programming languages on a single plot
* Smoothed trends using rolling averages

These plots help reduce noise and highlight meaningful long-term patterns.

---

## ▶️ How to Run

1. Clone this repository

2. Install dependencies:

   ```bash
   pip install pandas matplotlib
   ```

3. Place `QueryResults.csv` in the project directory.

4. Run the notebook:

   ```bash
   jupyter notebook
   ```

---

## 📌 Notes

* Some plots may appear duplicated if `DataFrame.plot()` is used alongside `plt.figure()`.
* Rolling averages help visualize trends but may hide short-term spikes.
* The y-axis is limited to improve readability of the plots.

---

## 📄 License

This project is for educational and exploratory purposes. Feel free to fork, modify, and build upon it.

---

## 🙌 Acknowledgments

* Stack Overflow for the dataset inspiration
* Pandas & Matplotlib open-source communities
