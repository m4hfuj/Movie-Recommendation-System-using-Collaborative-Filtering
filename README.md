# Movie Recommendation System using Collaborative Filtering

![Movie Recommendation](https://example.com/figure1.png)

## Tech Stack

<p align="center">
  <img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white" alt="Python">
  <img src="https://img.shields.io/badge/NumPy-013243?style=for-the-badge&logo=numpy&logoColor=white" alt="NumPy">
  <img src="https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white" alt="Pandas">
  <img src="https://img.shields.io/badge/Scikit--Learn-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white" alt="Scikit-learn">
  <img src="https://img.shields.io/badge/Matplotlib-11557C?style=for-the-badge&logo=matplotlib&logoColor=white" alt="Matplotlib">
  <img src="https://img.shields.io/badge/Seaborn-8FBC8F?style=for-the-badge" alt="Seaborn">
</p>

---

## Overview

This project implements a **Movie Recommendation System** using Collaborative Filtering techniques. By leveraging user and item interactions, the system predicts movie preferences for users, making personalized recommendations. The project is implemented in Python and utilizes essential libraries such as NumPy, Pandas, and Scikit-learn.

---

## Features

- **Collaborative Filtering**: Implements both user-based and item-based filtering.
- **Recommendation Prediction**: Predicts ratings for unrated movies based on user similarities.
- **Performance Metrics**: Includes evaluation metrics such as RMSE for validation.
- **Data Processing**: Handles large-scale movie-rating data efficiently.

---

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/Movie-Recommendation-System.git
   cd Movie-Recommendation-System
   ```

2. Install required packages:
   ```bash
   pip install -r requirements.txt
   ```

3. Run the Jupyter Notebook:
   ```bash
   jupyter notebook collaborative-filtering.ipynb
   ```

---

## Data Description

The dataset consists of the following:
- **Users**: Unique IDs for users.
- **Movies**: Unique IDs and metadata for movies.
- **Ratings**: Numerical ratings provided by users for specific movies.

Example Data Snapshot:
| User ID | Movie ID | Rating |
|---------|----------|--------|
| 1       | 101      | 5      |
| 2       | 102      | 3      |

---

## Methodology

### Collaborative Filtering

1. **User-Based Filtering**:
   - Measures similarity between users using cosine similarity.
   - Predicts ratings based on similar users' preferences.

2. **Item-Based Filtering**:
   - Measures similarity between items/movies.
   - Predicts ratings based on similar items.

### Evaluation

- **Root Mean Square Error (RMSE)**:
  - Computes the difference between predicted and actual ratings.
  - Formula:
    ![RMSE Formula](https://example.com/figure2.png)

---

## Key Functions

1. **Data Preprocessing**:
   - Handles missing values and normalizes ratings.
2. **Similarity Computation**:
   - Calculates cosine similarity between users and items.
3. **Recommendation Generation**:
   - Generates top-N recommendations for each user.

---

## Results

- **RMSE Performance**:
  - Achieved an RMSE of ~0.85 on the test set.
- **Top Recommendations**:
  - Example:
    - User 1: [Movie A, Movie B, Movie C]
    - User 2: [Movie D, Movie E, Movie F]

### Visualizations

#### User Similarity Matrix
![User Similarity Matrix](https://example.com/figure3.png)

#### Rating Distribution
![Rating Distribution](https://example.com/figure4.png)

---

## Future Improvements

- **Matrix Factorization**: Implement advanced techniques like SVD for better predictions.
- **Scalability**: Optimize for larger datasets.
- **Hybrid Methods**: Combine collaborative and content-based filtering.

---

## Contributing

Contributions are welcome! To contribute:
1. Fork the repository.
2. Create a new branch.
3. Commit your changes.
4. Submit a pull request.

---

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

---

## Acknowledgements

- MovieLens for providing the dataset.
- Open-source libraries that made this project possible.
