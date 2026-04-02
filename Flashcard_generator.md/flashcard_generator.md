import random
import re

# Sample study text (you can replace this with any notes or file input)
study_text = """
Python is a high-level programming language.
It supports object-oriented programming.
AI stands for Artificial Intelligence.
Machine Learning is a subset of AI.
"""

# Step 1: Extract key terms (simple regex for capitalized words or keywords)
def extract_keywords(text):
    # Split sentences
    sentences = text.strip().split("\n")
    flashcards = []
    for sentence in sentences:
        # Find keywords (capitalized words or important terms)
        keywords = re.findall(r'\b[A-Z][a-zA-Z]+\b', sentence)
        if keywords:
            question = f"What is {keywords[0]}?"
            answer = sentence
            flashcards.append((question, answer))
    return flashcards

# Step 2: Generate flashcards
flashcards = extract_keywords(study_text)

# Step 3: Quiz user
def quiz(flashcards):
    print(" Flashcard Quiz! Type your answer or press Enter to reveal.\n")
    for q, a in random.sample(flashcards, len(flashcards)):
        print(q)
        user_input = input("Your answer: ")
        print(f" Correct Answer: {a}\n")

quiz(flashcards)
