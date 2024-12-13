Here’s a polished write-up for your GitHub project:  

---

# **Flash Card GUI Application**  

A simple and intuitive GUI application designed to help users study any topic using flashcards. This program makes it easy to track progress and focus on areas that need improvement, ensuring a personalized and effective learning experience.  

---

## **How It Works**  

The application uses a CSV file to generate flashcards, following this format:  

```
topic_question,topic_answer  
question,answer  

Examples:  
Japanese,English  
私,"I, me"  
あなた,You  
```  
![](https://github.com/UnEvolvedGod/Flash-Cards/blob/main/images/answer_side.png)
### **Key Features**  

- **Customizable Study Topics**:  
  Import a CSV file with your topics and corresponding answers to tailor the flashcards to your needs.  

- **Progress Tracking**:  
  Incorrect answers are saved to a `words_to_learn.csv` file, allowing you to revisit and reinforce areas where you struggled.  

- **Dynamic Flashcard Interaction**:  
  - Flashcards display one at a time.  
  - The answer is revealed after 3 seconds.  
  - Users can mark their answers as correct or incorrect.  

- **Smart Restart**:  
  If the session ends prematurely, `words_to_learn.csv` retains all unanswered or incorrect items for future sessions.  

---

## **Program Workflow**  

1. **Starting the Program**:  
   - On launch, the program searches for an existing `words_to_learn.csv` file.  
   - If no such file exists, it defaults to the base list provided by the user.  

2. **Using Flashcards**:  
   - Flashcards appear sequentially, revealing the answer after a brief delay.  
   - Users choose whether their answer was correct or incorrect.  
   - Incorrect answers are saved to the `words_to_learn.csv` file for later review.  

3. **Session Completion**:  
   - The session continues until all flashcards are answered correctly, or the user manually ends it.  
   - Progress is saved if the session ends early.  

---

## **Important Notes**  

1. **Managing the `words_to_learn.csv` File**:  
   - If this file becomes empty, the program will not function correctly.  
   - To fix this, either delete the file to reset it or manually input words in the correct format.  

2. **Final Card Behavior**:  
   - On the last card, pressing "Check" before the answer is revealed may cause the congratulatory message to overlap with the final card’s definition.  

---

## **Getting Started**  

1. Clone the repository:  
   ```bash  
   git clone https://github.com/yourusername/flash-card-gui.git  
   ```  

2. Install the required dependencies:  
   ```bash  
   pip install -r requirements.txt  
   ```  

3. Run the application:  
   ```bash  
   python flash_card_gui.py  
   ```  

4. Prepare your CSV file following the specified format and enjoy learning!  

---

## **Future Improvements**  

- Add support for multimedia flashcards (e.g., images, audio).  
- Include a feature to adjust the answer reveal timer.  
- Improve UX for better navigation and error handling.  

---

Feel free to contribute, report issues, or suggest enhancements to make this tool even better! 😊  

--- 

Let me know if you'd like me to adjust anything!
