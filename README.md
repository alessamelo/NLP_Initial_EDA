# **Disaster Tweets — Exploratory Data Analysis (EDA)**

This notebook performs an exploratory data analysis (EDA) of the **Disaster Tweets** dataset. The objective is to understand the structural, lexical, and stylistic characteristics of tweets labeled as disaster-related or non-disaster-related.

The analysis focuses on:

* Dataset structure and missing values
* Text length statistics
* Metadata feature exploration
* Duplicate detection
* URL and emoji presence
* Preliminary linguistic signals

This EDA serves as the foundation for downstream NLP modeling.

---

##  Dataset Description

The dataset contains **7,613 tweets** with the following columns:

| Column     | Description                                   |
| ---------- | --------------------------------------------- |
| `id`       | Unique identifier                             |
| `keyword`  | Disaster-related keyword (optional)           |
| `location` | User-provided location (free text)            |
| `text`     | Tweet content                                 |
| `target`   | Binary label (1 = disaster, 0 = non-disaster) |

---

##  Technologies Used

* Python
* pandas
* matplotlib
* numpy
* emoji (for emoji detection)

---

##  Conclusion

This exploratory analysis highlights structural and stylistic differences between disaster and non-disaster tweets. While surface-level features offer limited separation, they provide valuable context for feature engineering and model design in subsequent NLP tasks.


