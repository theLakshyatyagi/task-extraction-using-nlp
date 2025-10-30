# Task Extraction using NLP
## Features
Extracts sentences from unstructured text

Identifies actionable tasks (e.g., “He has to buy snacks”)

Detects responsible person and deadlines

Categorizes each task into Work, Education, Personal, or Other

Outputs results in structured JSON format

## Technologies Used
Python 3

Regular Expressions (re)

JSON module

Jupyter Notebook / VS Code

## Project Structure
TaskExtraction.ipynb           → Main notebook

README.md                      → Project documentation

## How to Run
1. Open the notebook in Jupyter or VS Code
2. Run all cells sequentially
3. The final JSON output will show extracted tasks

## Example Input
Rahul wakes up early every day. He goes to college in the morning and comes back at 3 pm.
At present, Rahul is outside. He has to buy snacks for all of us.
The teacher asked students to complete their homework by tomorrow.
Neha must submit the report by Friday. Later, she will review the project.
Rohan is required to clean the lab by today.
The project should be completed by the end of the month.
By Next Monday, they will start a new assignment.

## Example Output
[
 {
 "task": "He has to buy snacks for all of us",
 "person": "He",
 "deadline": null,
 "category": "Personal Task"
 },
 {
 "task": "The teacher asked students to complete their homework by tomorrow",
 "person": "Teacher",
 "deadline": "tomorrow",
 "category": "Education"
 },
 {
 "task": "Neha must submit the report by Friday",
 "person": "Neha",
 "deadline": "Friday",
 "category": "Education"
 },
 {
 "task": "Later, she will review the project",
 "person": "She",
 "deadline": null,
 "category": "Work"
 },
 {
 "task": "Rohan is required to clean the lab by today",
 "person": "Rohan",
 "deadline": "today",
 "category": "Work"
 },
 {
 "task": "The project should be completed by the end of the month",
 "person": "The",
 "deadline": "the end of the month",
 "category": "Work"
 },
 {
 "task": "By Next Monday, they will start a new assignment",
 "person": "They",
 "deadline": "Next Monday",
 "category": "Education"
 }
]

## Future Improvements
Add Named Entity Recognition (NER) using spaCy

Use a trained ML model for better task categorization

Integrate with a web interface

## Author
Lakshya Tyagi
Delhi, India
