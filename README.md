# Twitter Sentiment Analysis 🐦

Sentiment analysis on a Twitter dataset, built as Task 4 of my Prodigy InfoTech internship. The goal: clean the data and explore how people feel about different topics and brands.

## 🛠️ Technologies
- **Python**
- **Pandas** and **NumPy** for data handling
- **Matplotlib** and **Seaborn** for charts
- **WordCloud** for text visuals
- **Google Colab / Jupyter Notebook**

## ✨ Features
- Data cleaning: removed missing values and duplicate rows
- Topic distribution chart showing which topics appear most
- Sentiment distribution as a count plot and a pie chart
- Topic vs sentiment comparison using a grouped count plot
- Separate bar charts of the top 5 topics for Negative, Positive, Neutral, and Irrelevant sentiment
- Sentiment breakdown for a single topic ("Google")
- Message length analysis with a histogram and a boxplot by sentiment
- Heatmap of Topic vs Sentiment
- Word cloud of topic names

## 🔄 The Process
1. Loaded `twitter_training.csv` and added column names (`ID`, `Topic`, `Sentiment`, `Text`)
2. Inspected the shape, data types, and unique sentiment labels
3. Cleaned the data by dropping nulls and duplicates
4. Plotted topic and sentiment distributions
5. Compared sentiment across topics, including the top 5 per sentiment
6. Added a `msg_len` column and compared message length across sentiments
7. Built a heatmap and word cloud to summarise the findings

## 📚 What I Learned
- **Data Cleaning:** Checking for nulls and duplicates before any analysis.
- **Categorical Analysis:** Using `groupby`, `value_counts`, and `crosstab` to compare categories.
- **Seaborn:** Building count plots, bar plots, boxplots, and heatmaps, and choosing colour palettes that fit the data.
- **Feature Engineering:** Creating a new column (`msg_len`) to find patterns in the text.
- **Choosing Charts:** Pie charts for proportions, boxplots for spread, heatmaps for two-way comparisons.
- **Reading Sentiment:** Turning raw tweets into insights about which topics get positive or negative reactions.

## 📁 Files
- `twitter_training.csv`: the dataset
- `prodigy_task_4.py`: the analysis script

## ▶️ How to Run
```bash
pip install pandas numpy matplotlib seaborn wordcloud
python prodigy_task_4.py
```
