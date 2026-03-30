# Text Autocomplete System

## Overview
This project is a Python-based text autocomplete system that predicts the next possible word based on previously entered text. The system is designed to simulate the basic working of predictive text models using simple logic and data structures instead of external machine learning libraries.

## Objective
The main objective of this project is to develop a system that:
- Suggests relevant next words based on input
- Learns dynamically from user input
- Updates predictions over time
- Demonstrates core machine learning concepts in a simplified manner

## Working Principle
The system uses a **bigram model**, where two consecutive words are used to predict the next word. It stores word pairs and tracks how frequently a particular word follows them.

For example:
If the dataset contains:
“I am going to college”  
“I am feeling happy”

The model learns that after “I am”, words like “going” and “feeling” are likely to appear. Based on frequency, it suggests the top three most probable words.

## Learning Mechanism
A key feature of this system is its ability to learn from user input. When new text is entered and trained:
- The model updates its internal data
- Word frequencies are increased
- Newly introduced words start appearing in suggestions

For instance:
Before training:
“I am → going | feeling | happy”

After training with:
“I am ironman”

Updated output may include:
“Ironman | going | feeling”

This demonstrates adaptive learning behavior.

## Features
- Predicts top 3 next-word suggestions
- Learns from user input in real time
- Updates predictions dynamically
- Simple graphical user interface
- Save and load functionality for model data

## User Interface
The system includes a GUI built using Tkinter, allowing users to:
- Enter text easily
- Generate suggestions with a button click
- Train the model with new data
- Save learned information for future use

## Implementation Details
The project is implemented using:
- Python (core language features)
- Dictionaries for storing word relationships
- Basic string processing for text cleaning
- JSON file handling for saving model data
- Tkinter for graphical interface

No external machine learning libraries are used, ensuring that the logic is built from scratch.

## Limitations
- Works only on a small dataset
- Uses only bigram (2-word) context
- Does not understand meaning, only frequency
- Prediction accuracy depends on training data

## Future Scope
- Implement trigram or higher-order models
- Improve prediction accuracy with larger datasets
- Add real-time typing suggestions
- Enhance user interface design

## Conclusion
This project demonstrates how a basic autocomplete system can be developed using simple programming concepts. It highlights how frequency-based models can simulate learning and prediction, forming the foundation for more advanced natural language processing systems.

## Author
Aryan Garg  
Registration Number: 25BAI10215
