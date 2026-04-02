Flashcard Generator with Basic AI
A simple Python project that generates study flashcards (Q&A pairs) using basic AI.
You can input raw text or notes, and the program will automatically create concise flashcards to help with learning and revision.

 Features
- Generate flashcards from any text or notes.
- AI-powered question-answer creation using OpenAI API (or GPT4All for offline use).
- Console-based interface for quick testing.
- Easily extendable to GUI (Tkinter/Streamlit).

Installation
- Clone the repository:
git clone https://github.com/your-username/flashcard-generator.git
cd flashcard-generator
- Install dependencies:
pip install openai

- Set your OpenAI API key:
export OPENAI_API_KEY="your_api_key_here"

- (On Windows PowerShell use: setx OPENAI_API_KEY "your_api_key_here")
   UsageRun the script:
  python flashcard_generator.py
  python flashcard_generator.py
   Flashcard Generator with AI
Enter your study material or notes: Photosynthesis is the process by which green plants use sunlight...
How many flashcards do you want? 3
output:
Q: What is photosynthesis?
A: The process by which green plants use sunlight to synthesize food from carbon dioxide and water.

Q: Which organisms primarily perform photosynthesis?
A: Green plants.

Q: What are the raw materials needed for photosynthesis?
A: Carbon dioxide and water.

Q: What is photosynthesis?
A: The process by which green plants use sunlight to synthesize food from carbon dioxide and water.

Q: Which organisms primarily perform photosynthesis?
A: Green plants.

Q: What are the raw materials needed for photosynthesis?
A: Carbon dioxide and water.
Q: What is photosynthesis?
A: The process by which green plants use sunlight to synthesize food from carbon dioxide and water.

Q: Which organisms primarily perform photosynthesis?
A: Green plants.

Q: What are the raw materials needed for photosynthesis?
A: Carbon dioxide and water.
