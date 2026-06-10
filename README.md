# 🤖 Text Summarizer Chatbot

A beginner-friendly Natural Language Processing (NLP) project built using Python and NLTK that summarizes long text into a short and meaningful summary. This chatbot helps users quickly understand the key points of articles, notes, reports, blogs, and documents without reading the entire content.

---

# 📌 Project Overview

Reading long paragraphs, articles, and documents can be time-consuming. The Text Summarizer Chatbot automatically extracts important sentences from the input text and generates a concise summary.

This project demonstrates the fundamentals of:

* Natural Language Processing (NLP)
* Text Processing
* Sentence Tokenization
* Python Programming
* Chatbot Development

---

# 🚀 Features

✅ Summarizes long text automatically

✅ Beginner-friendly project

✅ Fast text processing

✅ Works completely offline

✅ Easy to understand code

✅ No API Key Required

✅ No Internet Required After Setup

---

# 🛠️ Technologies Used

| Technology        | Purpose                     |
| ----------------- | --------------------------- |
| Python            | Programming Language        |
| NLTK              | Natural Language Processing |
| Punkt Tokenizer   | Sentence Splitting          |
| String Processing | Summary Generation          |

---

# 📂 Project Structure

```text
text-summarizer-chatbot/
│
├── app.py
├── requirements.txt
├── README.md
└── sample_text.txt
```

---

# ⚙️ Installation

## Step 1: Clone Repository

```bash
git clone https://github.com/yourusername/text-summarizer-chatbot.git
cd text-summarizer-chatbot
```

## Step 2: Install Dependencies

```bash
pip install nltk
```

## Step 3: Download Required NLTK Model

```python
import nltk
nltk.download('punkt')
```

---

# ▶️ Run The Project

```bash
python app.py
```

---

# 💻 Source Code

```python
import nltk
from nltk.tokenize import sent_tokenize

nltk.download('punkt')

print("🤖 Text Summarizer Chatbot")

while True:
    text = input("\nEnter Text: ")

    if text.lower() == "exit":
        break

    sentences = sent_tokenize(text)

    summary = " ".join(sentences[:3])

    print("\nSummary:")
    print(summary)
```

---

# 🔍 Complete Code Explanation

## 1. Import NLTK

```python
import nltk
```

### Purpose

NLTK (Natural Language Toolkit) is one of the most popular Python libraries for Natural Language Processing.

### Why Used?

* Text Processing
* Tokenization
* NLP Tasks
* Language Analysis

---

## 2. Import Sentence Tokenizer

```python
from nltk.tokenize import sent_tokenize
```

### Purpose

Converts a paragraph into individual sentences.

### Example

Input:

```text
SQL is a database language. It is widely used.
```

Output:

```python
[
 "SQL is a database language.",
 "It is widely used."
]
```

---

## 3. Download Punkt Tokenizer

```python
nltk.download('punkt')
```

### Purpose

Downloads the sentence tokenizer model required by NLTK.

Without this:

```text
LookupError: Resource punkt not found
```

may occur.

---

## 4. Display Welcome Message

```python
print("🤖 Text Summarizer Chatbot")
```

### Purpose

Shows a welcome message to the user when the chatbot starts.

---

## 5. Infinite Loop

```python
while True:
```

### Purpose

Allows the chatbot to run continuously until the user exits.

---

## 6. User Input

```python
text = input("\nEnter Text: ")
```

### Purpose

Accepts text from the user for summarization.

Example:

```text
Artificial Intelligence is changing the world...
```

---

## 7. Exit Condition

```python
if text.lower() == "exit":
    break
```

### Purpose

Stops the chatbot when the user enters:

```text
exit
```

---

## 8. Sentence Tokenization

```python
sentences = sent_tokenize(text)
```

### Purpose

Splits the paragraph into multiple sentences.

### Example

Input:

```text
AI is growing rapidly. It is used in healthcare.
```

Output:

```python
[
 "AI is growing rapidly.",
 "It is used in healthcare."
]
```

---

## 9. Summary Generation

```python
summary = " ".join(sentences[:3])
```

### Purpose

Selects the first three sentences and combines them into a summary.

### Breakdown

#### sentences[:3]

Selects:

```python
Sentence 1
Sentence 2
Sentence 3
```

#### join()

Combines selected sentences into a single paragraph.

Output:

```text
Sentence 1 Sentence 2 Sentence 3
```

---

## 10. Display Summary

```python
print("\nSummary:")
print(summary)
```

### Purpose

Displays the generated summary to the user.

---

# 🔄 Project Workflow

```text
User Input
     │
     ▼
Sentence Tokenization
     │
     ▼
Sentence Selection
     │
     ▼
Summary Generation
     │
     ▼
Display Output
```

---

# 📊 Example

## Input

```text
Artificial Intelligence (AI) is a branch of computer science that focuses on creating intelligent systems. AI is used in healthcare, education, cybersecurity, robotics, and many other fields. It helps automate tasks and improve decision-making. AI is rapidly growing and becoming an essential part of modern technology.
```

---

## Output

```text
Artificial Intelligence (AI) is a branch of computer science that focuses on creating intelligent systems. AI is used in healthcare, education, cybersecurity, robotics, and many other fields. It helps automate tasks and improve decision-making.
```

---

# 🎯 Applications

* Student Notes Summarization
* News Article Summarization
* Research Paper Summarization
* Blog Summarization
* Report Summarization
* Quick Revision Notes

---

# Advantages

* Saves Time
* Easy To Use
* Works Offline
* Fast Processing
* Beginner Friendly
* Minimal Dependencies

---

# Limitations

* Uses Extractive Summarization
* May Miss Important Context
* Does Not Generate New Sentences
* Not Suitable For Complex AI Summaries

---

# Future Improvements

* PDF Summarizer
* AI-Based Summarization
* Streamlit Web Application
* Voice Input Support
* Multi-Language Support
* Chat History Feature
* Document Upload Feature

---

# Time Complexity

### Sentence Tokenization

```text
O(n)
```

### Summary Extraction

```text
O(1)
```

### Overall Complexity

```text
O(n)
```

Where:

```text
n = Number of characters in input text
```

---

# Learning Outcomes

After completing this project, you will understand:

* Python Programming
* NLP Fundamentals
* NLTK Library
* Tokenization
* Chatbot Development
* Text Processing
* Software Project Documentation

---

# Resume Description

Developed a Text Summarizer Chatbot using Python and Natural Language Processing (NLP). The application processes user-provided text, extracts important information, and generates concise summaries to improve readability and reduce reading time.

---

# Author

**Ajay Sagar**

B.Tech CSE Student
Python Developer
AI & Machine Learning Enthusiast
