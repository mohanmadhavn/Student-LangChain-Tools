# Student-LangChain-Tools

A simple **LangChain Agent using Gemini** that answers student-related questions using tools and a SQLite database.

## What it can do

* Get student name and department
* Get student marks
* Calculate total and average marks
* Check university passing requirements

## Tools

* `get_student_info()` — returns name and department
* `get_student_marks()` — returns subject marks
* `calculator()` — performs calculations
* `get_passing_rules()` — returns passing criteria

## Technologies

* Python
* LangChain
* Gemini
* SQLite
* Google Colab

## How it works

```text
User Question
     ↓
Gemini Agent
     ↓
Selects required tools
     ↓
SQLite / Calculator
     ↓
Tool Results
     ↓
Final Answer
```

The agent decides which tools to use based on the user's question instead of following a fixed sequence.

## Example

```text
I am 22CS045. Tell me my name, department,
total marks, average marks, and whether I satisfy
the university passing requirements.
```

The agent automatically selects the required tools and generates the final answer.

## Passing Rules

* Minimum overall average: 40%
* Minimum mark in each subject: 35%

## Project Files

```text
student_agent.ipynb
students.db
requirements.txt
README.md
```
