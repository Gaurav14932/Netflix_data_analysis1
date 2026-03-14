# 🎬 Netflix Data Analysis

Exploratory Data Analysis (EDA) of Netflix movies and TV shows dataset to uncover trends in genres, popularity, release history, and audience ratings.

---

## 📌 Project Overview

This project performs a comprehensive EDA on a Netflix dataset containing metadata for **9,826 movies and TV shows**. The goal is to extract meaningful insights about content trends, audience preferences, and popularity patterns using Python and interactive visualizations.

---

## 📁 Project Structure

```
Netflix-Data-Analysis/
│
├── Netflix_Data_Analysis.ipynb   # Main Jupyter Notebook with full EDA
├── NetflixData.csv               # Dataset (place in /content/ if using Colab)
├── requirements.txt              # Python dependencies
└── README.md                     # Project documentation
```

---

## 📊 Dataset

**Source:** Netflix Movies & TV Shows Dataset (TMDB-based)

| Column | Description |
|---|---|
| `Release_Date` | Date the movie/show was released |
| `Title` | Title of the content |
| `Overview` | Short plot description |
| `Popularity` | TMDB popularity score |
| `Vote_Count` | Number of user votes |
| `Vote_Average` | Average user rating (0–10) |
| `Original_Language` | Language code (e.g., `en`, `fr`) |
| `Genre` | One or more genre labels |
| `Poster_Url` | URL to the movie poster image |

**Dataset Stats:**
- Rows: 9,826 | Columns: 9
- Popularity range: 13.35 – 5,083.95
- Vote average range: 0.0 – 10.0
- Release years span: 1902 – 2024
- 19 unique genres after preprocessing
- 43 unique original languages

---

## 🔍 Analysis Sections

### 1. Data Loading & Preview
Loading the dataset and previewing the first few rows to understand the structure.

### 2. Dataset Structure
Checking shape, column names, and data types using `.shape`, `.columns`, and `.info()`.

### 3. Statistical Summary
Descriptive statistics for numerical columns using `.describe()`.

### 4. Data Quality Check
- Identifying and counting duplicate rows
- Detecting missing values per column

### 5. Data Cleaning
- Removing 2 duplicate rows
- Dropping rows with missing values (~5 rows affected)

### 6. Data Preprocessing & Transformation
- Converting `Release_Date` to datetime and extracting the year
- Dropping irrelevant columns: `Overview`, `Poster_Url`, `Original_Language`
- Exploding the `Genre` column (multi-genre entries split into separate rows)

### 7. Feature Analysis & Visualization

| # | Question | Chart Type |
|---|---|---|
| 1 | Which genre appears most often? | Bar Chart |
| 2 | Which movies have the highest popularity? | Horizontal Bar Chart |
| 3 | How has movie production changed over time? | Line Chart |
| 4 | Which genres have the highest average popularity? | Bar Chart |
| 5 | What is the distribution of popularity scores? | Histogram |

---

## 💡 Key Insights

- **Drama** is the most common genre on Netflix.
- **Adventure** movies have the highest average popularity, followed by Action and Science Fiction.
- **Spider-Man: No Way Home** is the most popular movie in the dataset.
- Movie production grew **steadily after 2000**, peaking around 2017–2019.
- Popularity scores are **highly right-skewed** — most movies are average, with only a few becoming blockbuster hits.

---

## 🛠️ Technologies Used

- **Python 3**
- **Pandas** – Data manipulation and cleaning
- **Plotly Express** – Interactive visualizations
- **Google Colab** – Development environment

---

## 🚀 Getting Started

### Prerequisites

Install the required packages:

```bash
pip install -r requirements.txt
```

### Running the Notebook

**Option 1 – Google Colab (Recommended)**

1. Upload `Netflix_Data_Analysis.ipynb` to [Google Colab](https://colab.research.google.com/)
2. Upload `NetflixData.csv` to `/content/` in the Colab file browser
3. Run all cells

**Option 2 – Local Jupyter**

```bash
git clone https://github.com/YOUR_USERNAME/Netflix-Data-Analysis.git
cd Netflix-Data-Analysis
pip install -r requirements.txt
jupyter notebook Netflix_Data_Analysis.ipynb
```

> ⚠️ Update the file path in the notebook from `/content/NetflixData.csv` to your local path if running locally.

---

## 📬 Contact

Feel free to open an issue or connect via GitHub if you have any questions or suggestions!
# Netflix_data_analysis1
