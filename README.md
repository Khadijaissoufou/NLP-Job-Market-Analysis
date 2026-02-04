# 📊 Job Market Analysis for Data Professionals - NLP Project

## 🎯 Project Overview

This project performs **Natural Language Processing (NLP) analysis** on job postings for data-related internships and positions in France. Using text mining and statistical techniques, it extracts insights about:

- **Most demanded technical skills** (hard skills)
- **Most valued soft skills and qualities**
- **Top recruiting sectors**
- **Most sought-after job profiles**
- **Semantic clustering** of job descriptions

---

## 🛠️ Technologies & Tools

**Programming & Libraries:**
- Python 3.x
- Stanza (NLP pipeline for French language)
- Scikit-learn (TF-IDF, K-Means clustering)
- Pandas, NumPy (data manipulation)
- Matplotlib, Seaborn (data visualization)
- WordCloud (visual representation)
- NLTK (n-grams extraction)

**Data Processing:**
- Text preprocessing and cleaning
- Lemmatization and POS tagging
- Stopwords removal
- Regular expressions (regex)

---

## 🔍 Key Features

### 1. **Text Preprocessing**
- Removal of punctuation and special characters
- Lemmatization using Stanza NLP pipeline
- Filtering of stopwords, auxiliaries, and generic terms
- Part-of-speech (POS) tagging (verbs, nouns, adjectives)

### 2. **Hard Skills Extraction**
Automated detection of technical competencies including:
- Programming languages (Python, R, SQL, Java)
- Data tools (Tableau, Power BI, Excel, SAS)
- Frameworks & libraries (Pandas, TensorFlow, Scikit-learn, Spark)
- Cloud & DevOps (AWS, Azure, Git, Docker, Airflow)

**Output:** Word cloud + top 15 ranked skills by frequency

### 3. **Soft Skills Analysis**
Identification of personal qualities and behavioral competencies such as:
- Rigor, autonomy, curiosity, teamwork
- Communication, adaptability, analytical mindset

**Output:** Top 5 soft skills + word cloud visualization

### 4. **N-Grams Analysis**
Extraction of frequent word combinations:
- **Bigrams** (2-word phrases)
- **Trigrams** (3-word phrases)

Helps identify recurring expressions like "machine learning," "data analysis," "mise en place," etc.

### 5. **Sector Analysis**
Classification of job postings by industry using keyword matching:
- Banking & Insurance
- Healthcare
- Energy
- Tech / IT
- Retail
- Consulting
- Public sector

**Output:** Top 10 recruiting sectors

### 6. **Job Profile Identification**
Normalization and ranking of the most demanded positions:
- Data Analyst
- Data Scientist
- Data Engineer
- Business Analyst
- BI Consultant
- AI Engineer

**Output:** Top 10 job titles

### 7. **K-Means Clustering**
Semantic grouping of job postings using **TF-IDF vectorization** and **K-Means algorithm**:
- Elbow method to determine optimal number of clusters
- Lexical analysis of each cluster (top characteristic terms)

**Output:** Cluster distribution + lexical table

---

## 📊 Sample Outputs

### Hard Skills Word Cloud
![Hard Skills](https://via.placeholder.com/600x400?text=Hard+Skills+WordCloud)

### Top Recruiting Sectors
![Sectors](https://via.placeholder.com/600x400?text=Top+Sectors+Bar+Chart)

### Most Demanded Job Profiles
![Jobs](https://via.placeholder.com/600x400?text=Top+Jobs+Bar+Chart)

---

## 🚀 How to Run

### Prerequisites
```bash
pip install stanza pandas numpy matplotlib seaborn wordcloud nltk scikit-learn
```

### Download Stanza French Model
```python
import stanza
stanza.download('fr')
```

### Execute the Notebook
1. Upload your `Emploidata.txt` file (corpus of job postings)
2. Run all cells sequentially in the Jupyter notebook
3. View generated visualizations and statistics

---

## 📈 Key Insights

- **Python** and **SQL** are the most demanded technical skills
- **Rigor** and **autonomy** are the top soft skills
- **Tech/IT** and **Consulting** sectors recruit the most
- **Data Analyst** is the most frequent job title
- Clustering reveals distinct job families (technical vs. business-oriented)

---

## 🎓 Applications

This project is useful for:
- **Job seekers**: Understanding market demands and required skills
- **Career advisors**: Identifying trends in data professions
- **Recruiters**: Benchmarking job descriptions
- **Educators**: Adapting curricula to industry needs

---

## 👤 Author

**Khadija MAHAMADOU ISSOUFOU**  
Master's student in Data Science & Applied Economics  
University of Lille

📧 khadija.mahamadou19@gmail.com  
🔗 [LinkedIn](https://linkedin.com/in/khadija-mahamadou-issoufou)  
💻 [GitHub](https://github.com/Khadijaissoufou)

---

## 📝 License

This project is for educational and academic purposes.

---

## 🙏 Acknowledgments

- **Stanza NLP** by Stanford NLP Group
- **French Stopwords** by Gilles Bastin
- Data sources: Linkedin offers.
