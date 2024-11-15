# Book_Recommendation_System

This project aims to provide personalized book recommendations to users based on their reading preferences and ratings. The system utilizes collaborative filtering techniques to suggest books similar to those that users have rated highly.

## Table of Contents
1. [Introduction](#introduction)  
2. [Dataset Overview](#dataset-overview)  
3. [Data Preprocessing](#data-preprocessing)  
4. [Model Building](#model-building)  
5. [Results and Evaluation](#results-and-evaluation)  
6. [Usage](#usage)  
7. [Dependencies](#dependencies)  
8. [Contributor](#contributor)  

## Introduction  
The Book Recommendation System is designed to help users discover new books based on their past ratings and preferences. By analyzing user behavior and book ratings, the system can suggest books that similar users have enjoyed.

## Dataset Overview  
- **Dataset:** The dataset consists of three main files:
  - `Books.csv`: Contains details about books such as title, author, and ISBN.
  - `Users.csv`: Contains information about users.
  - `Ratings.csv`: Contains user ratings for books.

The data is loaded from text files and merged to create a comprehensive dataset for analysis.

## Data Preprocessing  
The following preprocessing steps are performed on the dataset:
1. **Loading Data**: The dataset is loaded using pandas.
2. **Merging Data**: Ratings are merged with book details to associate user ratings with book information.
3. **Filtering Users**: Users who have rated more than 50 books are filtered for more reliable recommendations.
4. **Filtering Books**: Books that have been rated at least 10 times are considered for recommendations.

## Model Building  
The recommendation model is built using the following steps:
1. **Creating a Pivot Table**: A pivot table of ratings is created to represent users' ratings for each book.
2. **Building the Recommendation Model**: A Nearest Neighbors model is used to find similar books based on user ratings.
3. **Recommendation Function**: A function is created to recommend books based on a user's input.

## Results and Evaluation  
The system provides recommendations based on the similarity of book ratings among users. Users can input a book title, and the system will return a list of recommended books that are similar in nature.

## Usage  
To use this project:
1. Clone this repository to your local machine.
2. Ensure you have all dependencies installed.
3. Run the Jupyter Notebook provided in this repository to execute the code and see results.

## Dependencies  
To run this project, ensure you have the following libraries installed:
- Python 3.11
- pandas
- numpy
- sklearn

You can install these packages using pip:

```bash
pip install pandas numpy scikit-learn
```
## Contributor
**Tejas Sinroja**: Project development, model design, and implementation.
- Feel free to contribute by suggesting improvements or reporting issues via GitHub!
