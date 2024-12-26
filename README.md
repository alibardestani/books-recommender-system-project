# Book Recommender System

A machine learning-based system to recommend books to users based on their preferences and similar user ratings. This project uses collaborative filtering and the Nearest Neighbors algorithm for personalized recommendations.

---

## Features
- **Data Processing**: Preprocessed datasets for books, users, and ratings.
- **Book Recommendation**: Suggests similar books using user ratings.
- **Interactive Functionality**: Easily search for a book and get recommendations.
- **Model Artifacts**: Includes trained models and serialized data for reuse.

---

## Datasets
The system uses the following datasets:
1. **Books**: Contains book titles, authors, publishers, and image URLs.
2. **Users**: Information about users who rated books.
3. **Ratings**: Book ratings provided by users.

---

## How It Works
1. **Data Preprocessing**:
   - Cleaned and structured datasets.
   - Filtered active users and books with significant ratings.
2. **Model Training**:
   - Built a pivot table of book ratings.
   - Trained a Nearest Neighbors model using the sparse representation of the data.
3. **Recommendations**:
   - Input a book name to get a list of similar books based on user preferences.

---

## Example Usage

```python
# Import the recommendation function
from recommend import recommend_book

# Provide a book name
book_name = "Harry Potter and the Chamber of Secrets (Book 2)"

# Get recommendations
recommend_book(book_name)
```
