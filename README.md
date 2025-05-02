# 🚖 Uber Demand & Supply Analysis with PySpark

This data engineering project leverages a real-world dataset from Uber to explore patterns in ride requests, driver supply, and trip completions using **PySpark**, a powerful big data processing library in Python.

## 📂 Dataset

The dataset used in this project is a real-world Uber dataset stored in CSV format. It contains hourly-level data over a two-week period and includes key metrics such as:
- Rider requests (eyeballs)
- Completed trips
- Available drivers
- Timestamps (hourly)

We'll load the dataset into a PySpark DataFrame and perform various data transformations and analyses to uncover valuable insights into Uber's demand and supply dynamics.

## 🎯 Project Objective

The goal of this project is to:
- Practice PySpark skills in a real-world context
- Perform data cleaning, transformation, and exploratory analysis
- Gain insights into Uber’s demand-supply mechanics
- Answer key analytical questions relevant to data engineering

This project also serves as a great **take-home assignment** or learning tool for those getting started with **PySpark** and **Data Engineering** concepts.

## ❓ Key Analytical Questions

Throughout the project, we aim to answer the following questions:

1. **Which date had the most completed trips during the two-week period?**
2. **What was the highest number of completed trips within a 24-hour period?**
3. **Which hour of the day had the most ride requests during the two-week period?**
4. **What percentage of all zeroes (unfulfilled requests) occurred during the weekend (Friday 5 PM – Sunday 3 AM)?**  
   *Tip: The `hour` field represents the start of the hour.*
5. **What is the weighted average ratio of completed trips per driver during the two-week period?**  
   *Tip: Use trip volume as weights for an accurate average.*
6. **What are the busiest 8 consecutive hours (same each day) for scheduling driver shifts based on unique rider requests?**  
   *Shifts repeat every 8 hours; the goal is to optimize driver scheduling.*
7. **True or False: Driver supply always increases when demand increases during the two-week period?**  
   *Tip: A visual exploration can help answer this.*
8. **Which 72-hour window has the highest ratio of unfulfilled requests (Zeroes) to total rider requests (Eyeballs)?**
9. **If you could add 5 drivers to one hour every day, which hour should you choose?**  
   *Hint: Consider both unmet demand and current driver supply.*
10. **What time of day best represents the natural “end of day,” where both supply and demand are at their lowest?**

## 🛠️ Tools & Technologies

- Python 🐍
- PySpark ⚡
- Pandas (for optional pre-processing)
- Matplotlib / Seaborn (for visualizations)
- Jupyter Notebook / Databricks Notebook

## 🚀 Getting Started

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/uber-demand-supply-analysis.git
   cd uber-demand-supply-analysis
   ```

2. Install required packages:
   ```bash
   pip install pyspark pandas matplotlib seaborn
   ```

3. Open the notebook and follow the steps to explore and analyze the dataset.

## 📈 Visual Insights

Visualizations are used throughout the analysis to better understand demand trends, supply fluctuations, unmet requests, and optimal scheduling periods.

## 🤝 Contributing

Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

## 📄 License

[MIT](LICENSE)
