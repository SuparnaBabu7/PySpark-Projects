# 🎬 Indian Box Office Analysis with PySpark in Microsoft Fabric

## 📌 About the Project

This project focuses on analyzing Indian Box Office performance using PySpark within the **Microsoft Fabric** environment. The objective is to derive meaningful insights from a comprehensive film dataset spanning over the last 10 years. This includes details like film title, industry, release timeline, collections, OTT presence, ratings, and more.

Leveraging Microsoft Fabric’s **Lakehouse** and **Notebook** capabilities along with **PySpark**, this analysis aims to assist stakeholders in making data-driven decisions in the entertainment industry.

---

## 🧩 Problem Statement

The Indian Box Office dataset contains detailed information about movies released in the last decade. The goal of this project is to:
- Clean and prepare raw datasets using PySpark
- Integrate data across multiple dimensions (genre, language, director)
- Perform advanced analysis on box office collections
- Generate insights for key business questions in the film industry

---

## 🗃️ Datasets Used

- `Boxoffice.csv`  
- `Director.csv`  
- `Genre.csv`  
- `Language.csv`  

These datasets were ingested and processed using Microsoft Fabric's **Lakehouse** and analyzed via **PySpark** notebooks.

---

## 🛠️ Tech Stack

- 💻 **PySpark**  
- 📊 **Microsoft Fabric Notebook**  
- ☁️ **Microsoft Fabric Lakehouse**  
- 🧠 **DataFrames, Joins, Aggregations, and Filtering**  
- 🧹 **Data Cleaning and Feature Engineering**  

---

## 🧾 Dataset Descriptions

### 🔹 Boxoffice_Fact
| Column | Description |
|--------|-------------|
| FilmID | Unique identifier for each film |
| Title | Film title |
| Release Date | Date of release |
| Lead Actor/Actress | Main cast |
| Industry | Film industry (e.g., Bollywood, Tollywood) |
| Budget in Crores | Production budget in INR |
| First Day Collection Worldwide | First-day worldwide revenue |
| Worldwide Collection | Total global box office |
| Overseas Collection | Earnings from overseas markets |
| India Gross Collection | Domestic gross earnings |
| Verdict | Film's success label (e.g., Hit, Flop) |
| IMDb Rating | IMDb rating score |
| Runtime (mins) | Duration of the film |
| OTT Platform | Streaming platform availability |
| DirectorID | Foreign key linking to Director_dim |
| LanguageID | Foreign key linking to Language_dim |
| GenreID | Foreign key linking to Genre_dim |

### 🔹 Director_dim
| Column | Description |
|--------|-------------|
| DirectorID | Unique ID for each director |
| Director | Name of the director |

### 🔹 Language_dim
| Column | Description |
|--------|-------------|
| LanguageID | Unique ID for each language |
| Language | Language of the film |

### 🔹 Genre_dim
| Column | Description |
|--------|-------------|
| GenreID | Unique ID for each genre |
| Genre | Film genre (e.g., Action, Drama) |

---

## 🔍 Steps Performed

1. **Workspace Setup**  
   - Created Microsoft Fabric workspace and configured capacity

2. **Data Ingestion**  
   - Uploaded `.csv` datasets to the Lakehouse  
   - Verified schema and ensured consistency

3. **Notebook Development with PySpark**  
   - Created a Fabric Notebook and initialized Spark session  
   - Read data using `spark.read.csv()` and applied schema inference

4. **Data Cleaning**  
   - Removed:
     - Special characters
     - Nulls and duplicates
     - Leading/trailing spaces in string columns

5. **Data Analysis & Joins**  
   - Joined fact and dimension tables using foreign keys  
   - Analyzed KPIs like:
     - Top-grossing genres and languages  
     - Directors with most hits  
     - IMDb vs. collection correlations  
     - OTT availability patterns

6. **Insight Delivery**  
   - Shared cleaned, aggregated tables with stakeholders  
   - Enabled downstream visualization in Power BI (optional)

---

## 📈 Outcome

This end-to-end analysis demonstrates the efficiency of using **Microsoft Fabric + PySpark** for handling complex entertainment datasets. It highlights how modern cloud platforms can simplify traditional ETL + analytics workflows — helping decision-makers gain faster and deeper insights.

---

## 📌 Project done by

**Inturi Suparna Babu**  
🔗 [Connect with me on LinkedIn](https://www.linkedin.com/in/inturi-suparna-babu-312b59270/)  
  
