# 🎓 Intelligent Recommendation System for E-Learning Platforms

A content-based course recommendation system that suggests relevant online courses to learners based on their interests, using TF-IDF vectorization and Cosine Similarity.

![Python](https://img.shields.io/badge/Python-3.10-blue)
![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-150458)
![Scikit-learn](https://img.shields.io/badge/Scikit--learn-ML-F7931E)
![License](https://img.shields.io/badge/License-MIT-green)

---

## 📌 Table of Contents

- [Overview](#-overview)
- [Problem Statement](#-problem-statement)
- [Features](#-features)
- [Tech Stack](#-tech-stack)
- [Dataset](#-dataset)
- [System Workflow](#-system-workflow)
- [Installation](#-installation)
- [Usage](#-usage)
- [Results](#-results)
- [Project Structure](#-project-structure)
- [Limitations](#-limitations)
- [Future Scope](#-future-scope)
- [Conclusion](#-conclusion)
- [License](#-license)

---

## 🧾 Overview

E-learning platforms host thousands of courses, making manual course discovery time-consuming and inefficient. This project implements an **Intelligent Recommendation System** that takes a student's interest as natural-language text (e.g., *"Python and Data Analysis"*) and returns the top 5 most relevant courses — along with category, difficulty level, and average rating.

The system uses **Content-Based Filtering**, powered by **TF-IDF** text vectorization and **Cosine Similarity**, to match user interests with course content.

---

## ❓ Problem Statement

With growing course catalogs on e-learning platforms, students struggle to find courses matching their specific interests among hundreds of options across categories and difficulty levels. This leads to wasted time, poor course selection, and reduced learner engagement. This project addresses that gap by automating relevant course discovery.

---

## ✨ Features

- 🔍 Natural-language interest input (e.g., "Web Development and Design")
- 🎯 Top 5 personalized course recommendations
- 📊 Exploratory Data Analysis of course categories, ratings, and difficulty
- 🧮 Evaluation via category-match precision metric
- 💬 Interactive command-line style interface (Google Colab)
- ⚠️ Graceful handling of vague or unrelated queries

---

## 🛠 Tech Stack

| Category | Tools |
|---|---|
| Language | Python 3.10 |
| Environment | Google Colab |
| Data Handling | Pandas, NumPy |
| Visualization | Matplotlib, Seaborn |
| Machine Learning | Scikit-learn (TF-IDF, Cosine Similarity) |

---

## 📂 Dataset

- **Type:** User-course interaction log (transactional dataset)
- **Size:** 8,000 interaction records × 26 features
- **Unique Courses:** 40
- **Unique Users:** 1,492
- **Categories:** Programming, Data Science, Marketing, Business, Design, Language Learning, Mathematics, Personal Development

Key columns include `course_name`, `course_category`, `course_difficulty`, `course_rating`, `completion_percentage`, and user demographic details.

---

## 🔄 System Workflow

```
Raw Dataset → Data Cleaning → EDA → Feature Aggregation (Course-Level)
    → Text Preprocessing (tags column) → TF-IDF Vectorization
    → Cosine Similarity → Recommendation Function
    → Testing & Evaluation → Interactive Interface
```

---

## ⚙️ Installation

```bash
git clone https://github.com/<your-username>/intelligent-recommendation-system-elearning.git
cd intelligent-recommendation-system-elearning
pip install -r requirements.txt
```

**requirements.txt**
```
pandas
numpy
matplotlib
seaborn
scikit-learn
```

---

## ▶️ Usage

1. Open `notebooks/Intelligent_Recommendation_System.ipynb` in Google Colab.
2. Run all cells sequentially.
3. When prompted, enter your interest, e.g.:

```
Enter your interest (e.g., 'Python and Data Analysis'): Python and Data Analysis
```

4. The system returns the top 5 recommended courses with category, difficulty, and rating.

---

## 📈 Results

- Achieved an average **category-match precision of ~80–85%** across test cases.
- Successfully handled clear, vague, and unrelated queries without errors.
- Delivered consistent, relevant recommendations across all 8 course categories.

---

## 📁 Project Structure

```
intelligent-recommendation-system-elearning/
│
├── README.md
├── requirements.txt
├── data/
│   └── dataset.csv
├── notebooks/
│   └── Intelligent_Recommendation_System.ipynb
└── docs/
    └── project_report.pdf
```

---

## ⚠️ Limitations

- Small course catalog (40 courses) limits recommendation diversity.
- No explicit user feedback available; evaluation relies on a proxy metric (category-match precision).
- Does not yet incorporate individual user history or learning style into recommendations.

---

## 🚀 Future Scope

- Combine with **Collaborative Filtering** for a hybrid recommendation approach.
- Incorporate richer course descriptions for improved TF-IDF matching.
- Deploy as a web application (e.g., using Streamlit or Flask).
- Scale to larger datasets using dimensionality reduction (e.g., Truncated SVD).

---

## ✅ Conclusion

This project demonstrates that a lightweight, interpretable **Content-Based Filtering** approach — using TF-IDF and Cosine Similarity — can effectively power a functional course recommendation system without requiring complex deep learning models or extensive user history. It successfully meets its objective of transforming natural-language interest into relevant, ranked course suggestions, offering a practical foundation for smarter course discovery on e-learning platforms.

---

## 📜 License

This project is licensed under the MIT License.

---

## 🙋 Author

**Dhananjay Emoliya**
[LinkedIn](https://www.linkedin.com/in/dhananjay-emoliya-609568333/) • [GitHub](https://github.com/dhananjayemoliya-code) • [Email](dhananajayemoliya@gmail.com)
