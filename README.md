# FAQ Bot with Similarity Scoring in Pure Python

## Project Overview

This FAQ Bot project allows users to upload their training dataset in CSV format to create an intelligent Frequently Asked Questions bot. It leverages similarity scoring models, including cosine, Jaccard, and TF-IDF, to identify the most relevant answers from the training dataset based on the user's questions. Written in pure Python and utilizing only essential libraries like csv, math, and Pandas, this project is the first in a series aimed at learning the construction of recommendation systems.

## How It Works

The process of answering a user's question involves several steps:

1. **Upload Training Data**: Users start by uploading their FAQ dataset in a CSV format.
2. **Remove Stop Words**: The application cleans the data by removing stop words to enhance the similarity matching process.
3. **Create DataFrame**: The cleaned data is converted into a Pandas DataFrame for easier manipulation and analysis.
4. **Vectorize Questions with Weighted Question Words**: Questions in the training data are vectorized with an emphasis on significant words to improve match accuracy.
5. **Get User’s Question**: The system prompts the user to input their question.
6. **Vectorize the User’s Question**: The user's question is then vectorized in the same manner as the training questions.
7. **Calculate Similarity Scores**: The application calculates the similarity scores between the user's question and the training questions using cosine, Jaccard, and TF-IDF methods.
8. **Check for Consensus**: It checks if at least two similarity scores match to identify the most optimal corresponding question. If there's no consensus, the bot returns "I don’t know."
9. **Search the DataFrame for the Matching Question**: Once a match is identified, the system searches the DataFrame for the corresponding question.
10. **Print the Answer**: The answer related to the identified question is displayed to the user.
11. **Prompt for Another Question**: The user is then encouraged to ask another question, continuing the interaction.



