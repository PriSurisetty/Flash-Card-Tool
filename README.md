# Flashcard Language Learning App:

This is a simple flash card application built with Python and Tkinter, designed to help users learn and memorize French vocabulary. 
The app presents a French word and, after a brief delay, reveals its English translation. Users can mark words they know, and the app will 
keep track of which words need further review.

## Features:

- **Interactive Flash Cards**: Displays a French word on the front side and its English translation on the back after 3 seconds..
- **Word Management**: Keeps track of words that need to be learned. Words marked as "known" are removed from the learning list.
- **Data Persistence**: Stores progress in a CSV file, ensuring that known words are not shown again in future sessions.
- **User-Friendly UI**: Simple and intuitive graphical interface using Tkinter.

## Prerequisites:

- **Python 3.x**
- **pandas**: For handling CSV files.
- **Tkinter**: For creating the graphical user interface.

## Installation:

1. **Clone the repository**:

   ```bash
   git clone <repository-url>

2. **Navigate to the project directory**:
   ```bash
   cd <project-directory>

3. **Install the required Python libraries**:
   ```bash
   pip install pandas

## Usage:

- **Run the application**:

  ```bash
  python main.py


## How It Works##:
- Word Generation: The app randomly selects a French word from a dataset (french_words.csv). If a file named words_to_learn.csv exists, the app loads this file instead, allowing users to continue from where they left off.
- Data Management with pandas: The pandas library is used to read, write, and manipulate the word data stored in CSV files, ensuring efficient data handling.
- Card Flipping: After 3 seconds, the flash card flips to show the English translation of the French word.
- Known Words: If a user knows a word, they can mark it as known, and it will be removed from the list of words to study. The updated list is saved to words_to_learn.csv using pandas.

