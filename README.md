# 🎬 Netflix Data Cleaning & Preprocessing Project

Welcome to the **Data Analyst Internship Task 1**, where the mission was simple (but critical):  
> **Turn a messy Netflix dataset into a clean, analysis-ready gem.**

This project focuses on **cleaning and preprocessing the Netflix Titles dataset** using **Python (Pandas)** in **Google Colab**.

---

## 🧠 Objective

> Clean and prepare a raw dataset by handling:
- Missing values  
- Duplicates  
- Inconsistent text formatting  
- Improper data types  
- Unstandardized column names

---

## 📊 Dataset Used

- 📁 **Netflix Movies and TV Shows**
- 📌 Source: [Kaggle Dataset](https://www.kaggle.com/datasets/shivamb/netflix-shows)
- 🔢 Rows: 8,807 | 📈 Columns: 12

---

## 🚀 Key Cleaning Steps

1. **Removed duplicates** to ensure unique titles.
2. **Filled missing values**:
   - `country` → "Unknown"
   - `rating` → "Not Rated"
   - `director`, `cast` → "Not Available"
   - `date_added` → Forward-filled using `.ffill()`
3. **Converted**:
   - `date_added` → `datetime` format
4. **Standardized text**:
   - Lowercased and stripped spaces in column names.
5. **Renamed columns** to snake_case for consistency.
6. **Final Export**: Saved as `netflix_titles_cleaned.csv`.

---

## 🔍 Preview of Cleaned Dataset

Here’s a glimpse of the cleaned data. Notice the NaNs waiting to be replaced and the general structure pre-cleanup.

![Cleaned Dataset]("Screenshot%%2025-06-23%130642.png")

---

## 🧾 Dataset Info Summary

No more missing values — just clean, tight data ready for analysis.

![Dataset Info]("Screenshot%2025-06-23%130657.png")

---

## 📊 Netflix Content Distribution

TV Shows and Movies face off in this pie chart.  
Turns out, Netflix *is* still more about movies!

![Netflix Content Pie Chart]("Screenshot%2025-06-23%130706.png")

---

## 💡 Creative Twist: The Netflix Cleanup Saga

> *"Not all heroes wear capes. Some of us wield Pandas."*

Netflix nearly recommended me:
- A show from "nan" directed by "Not Available",
- Released on a day lost to the void,
- Tagged as `[no genre, just vibes]`.

So I took out my data mop and got to work.  
What followed was a digital decluttering — Marie Kondo would be proud.

---

## 📁 Files in this Repository

| File Name                     | Description                                    |
|------------------------------|------------------------------------------------|
| `netflix_cleaning.ipynb`     | The full Colab notebook with code + comments  |
| `netflix_titles_cleaned.csv` | The final cleaned dataset                     |
| `summary.txt`                | Brief summary of changes made                 |
| Screenshots (.png)           | Visuals of dataset and charts                 |

---

## 👩‍💻 Tools & Tech

- Python 🐍  
- Pandas 📊  
- Google Colab 🧠  
- Matplotlib 

---

## 🔗 How to Use

```bash
1. Clone the repo
2. Open netflix_cleaning.ipynb in Google Colab
3. Run the notebook
4. Use the cleaned CSV for any analysis/ML projects

