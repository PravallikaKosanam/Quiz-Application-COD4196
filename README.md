Title: CodTech IT Solutions Internship - Task Documentation: Quiz Application*
**Introduction:**
This document provides a detailed explanation of the task assigned during the Codtech IT Solutions internship program. The task involves writing a python program to Design a quiz that challenges users with multiple-choice questions from various categories. Store questions and answersin lists or dictionaries, track scores, and provide feedback on results. Additionally it will include information about the intern, Pravallika Kosanam, and assigned ID,COD4196.
**Intern Information:**
Name: Pravallika Kosanam
Intern: COD4196
**Task Description:**
The task assigned to -Pravallika Kosanam during the CodTech IT Solutions internship program is to write a Quiz Application that that challenges users with multiple-choice questions from various categories. Store questions and answersin lists or dictionaries, track scores, and provide feedback on results. Below is the code implementation:
'''python
class PythonQuiz:
    def __init__(self):
        self.questions = {
            "Basics": {
                "What is the output of the following code snippet?\nprint(2 + 2 * 3)": ["A. 8", "B. 10", "C. 6", "D. 12"],
                "What is the correct way to declare a variable in Python?": ["A. variable x", "B. x = 5", "C. x := 5", "D. x 5"],
                "Which of the following is not a valid data type in Python?": ["A. String", "B. Dictionary", "C. Tuple", "D. Array"]
            },
            "Functions": {
                "What keyword is used to define a function in Python?": ["A. define", "B. function", "C. def", "D. fun"],
                "What does the 'return' statement do in a function?": ["A. Exits the function", "B. Returns a value from the function", "C. Defines a loop", "D. Prints a value"]
            },
            "Modules": {
                "Which module in Python is used for regular expression?": ["A. regex", "B. re", "C. regexpy", "D. regexlib"],
                "How do you import a module named 'example_module' in Python?": ["A. include example_module", "B. from example_module import *", "C. import example_module", "D. import * from example_module"]
            }
        }
        self.score = 0

    def start_quiz(self):
        print("Welcome to the Python Quiz!")
        for category, questions in self.questions.items():
            print("\nCategory:", category)
            for question, options in questions.items():
                print("\n", question)
                for option in options:
                    print(option)
                answer = input("Enter your answer (A/B/C/D): ").upper()
                correct_answer = options[0]
                if answer == correct_answer[0]:
                    print("Correct!")
                    self.score += 1
                else:
                    print("Incorrect! The correct answer is:", correct_answer)
        print("\nQuiz Complete!")
        print("Your Score:", self.score, "/", len(self.questions) * len(self.questions["Basics"]))

if __name__ == "__main__":
    quiz = PythonQuiz()
    quiz.start_quiz()
**Code Explanation:**
The Python quiz application is implemented using a class named PythonQuiz.
Inside the class, questions are organized into a dictionary structure where each category contains multiple questions with their corresponding options.
The start_quiz() method initiates the quiz by iterating over each category and presenting its associated questions to the user.
For each question, the user is prompted to enter their answer, and the code validates the response against the correct answer.
The user's score is incremented for each correct answer.
After all questions have been answered, the quiz concludes by displaying the user's final score and providing feedback on their performance.
**Rationale:**
Python quiz code is rationalized by its effectiveness in providing an interactive, engaging, and educational experience for users interested in testing and improving their knowledge of Python programming language. Through its structured organization, interactivity, educational value, scalability, and user-friendly design, the quiz serves as a valuable learning tool for Python enthusiasts of all levels.
**Conclusion:**
In conclusion the task assigned to Pravallika Kosanam during the CodTech IT Solutions internship program involved writing a python program to create a Quiz Application. the Python code for the quiz application provides a well-structured, interactive, and educational platform for users to test and improve their knowledge of Python programming language. This documentation provides insights into the implementation details, code explanation, and rationale behind the chosen approach. Pravallika Kosanam, with the intern ID COD4196, has effectively completed this task as part of the internship program.
This concludes the documentation for the task "Quiz Application" assigned during the CodTech IT Solutions internship program.









