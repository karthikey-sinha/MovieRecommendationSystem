
#  Netflix Movie RecommendationSystem

A simple yet effective content-based recommendation system built using **Python**, **Pandas**, **Scikit-learn**, and **NLTK**.
This project recommends Netflix titles based on their **genre similarity** using **TF-IDF vectorization** and **cosine similarity**.

---

##  Features

* Cleans and preprocesses Netflix metadata.
* Uses natural language processing to stem and remove stopwords.
* Calculates similarity between titles using TF-IDF.
* Recommends top 10 similar Netflix shows/movies for a given title.

---

##  How It Works

1. **Load Dataset**
   Read `netflixData.csv` containing metadata like Title, Description, Content Type, and Genre.

2. **Preprocessing**

   * Converts text to lowercase.
   * Removes HTML tags, URLs, punctuation, and digits.
   * Removes stopwords and applies stemming using NLTK.

3. **Vectorization**

   * Applies TF-IDF vectorizer on the `Genres` column.
   * Converts text into numerical vectors.

4. **Similarity Computation**

   * Uses **cosine similarity** to compare genre vectors between titles.

5. **Recommendation Function**

   * Returns top 10 titles similar to the input Netflix title.

---

##  Installation

Install the required Python packages:

```bash
pip install nltk scikit-learn pandas
```

Download NLTK stopwords:

```python
import nltk
nltk.download('stopwords')
```

---

##  Usage

1. Make sure `netflixData.csv` is in the project directory.
2. Run the script or import the function into your Python environment.

```python
netflix_recommendation("fitoor")
```

Sample Output:

```
0    fitoor

...
```

---

## Dataset Columns Used

* **Title** – Name of the show/movie.
* **Description** – Summary (used for cleaning context).
* **Content Type** – Movie/TV Show.
* **Genres** – Used for similarity calculation.

---

##  Example: Text Cleaning

Before:

```
"This is a beautifully crafted romantic drama, with emotional highs and lows."
```

After:

```
"beauti craft romant drama emot high low"
```

---

##  Dependencies

* `pandas`
* `scikit-learn`
* `nltk`
* `numpy`

---

## Author

Your Name
Karthikey Sinha



