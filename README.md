# 🎬 Movie Recommendation System (Content-Based Filtering)

This project implements a **Content-Based Movie Recommendation System** using **movie genres** and **cosine similarity**.  
It recommends movies similar to a given movie based on genre similarity and visualizes the recommendations using multiple graphs.

---

## 📌 Project Highlights

- Content-Based Filtering (No ratings required)
- Genre-based similarity using NLP
- Memory-optimized cosine similarity computation
- 10+ insightful data visualizations
- Suitable for academic projects & internships

---

## 📂 Dataset

- **movies.csv**
- Columns:
  - `movieId`
  - `title`
  - `genres`

📌 Dataset contains **no ratings**, so **content-based filtering** is the correct approach.

---

## 🛠️ Technologies Used

- Python
- Pandas
- NumPy
- Scikit-learn
- Matplotlib
- Seaborn
- Jupyter Notebook

---

## ⚙️ Project Workflow

1. Load and preprocess movie data  
2. Convert genres into numerical vectors using `CountVectorizer`  
3. Compute cosine similarity dynamically (memory-efficient)  
4. Recommend top N similar movies  
5. Visualize recommendations using multiple graphs  

---

## 🧠 Recommendation Logic

- Each movie’s genres are converted into a vector
- Cosine similarity measures similarity between genre vectors
- Similarity is computed **only for the selected movie**
- Prevents memory overflow for large datasets

📌 **Why not full similarity matrix?**

> Computing a full N×N cosine similarity matrix requires O(n²) memory.  
> To optimize memory usage, similarity is computed dynamically for the selected movie only.

---

## ▶️ How to Run the Project

### 1️⃣ Clone Repository
```bash
git clone https://github.com/yourusername/movie-recommendation.git
cd movie-recommendation
