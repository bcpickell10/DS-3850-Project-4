# DS-3850-Project-4
This repository holds my class projects from DS 3850, which have been re-created with ChatGPT 3.5.

# Quiz
    def run_quiz():
    # Introduction
        print("Welcome to the Python Quiz!\nAnswer the following questions:")

    # Define the quiz questions and answers using a dictionary
        questions = [
         {
            "question": "What is the capital of France?",
            "choices": ["A. Paris", "B. London", "C. Berlin", "D. Rome"],
            "answer": "A"
        },
        {
            "question": "Python is a high-level programming language. (True/False)",
            "answer": "True"
        },
        {
            "question": "What is the largest mammal?",
            "answer": "Blue whale"
        },
        {
            "question": "Which of the following is not a Python data type?",
            "choices": ["A. List", "B. Tuple", "C. Dictionary", "D. Array"],
            "answer": "D"
        },
        {
            "question": "The capital of Spain is ____________.",
            "answer": "Madrid"
        }
    ]

    # Initialize score counter
        score = 0

    # Iterate through each question
        for index, question in enumerate(questions, start=1):
            print(f"\nQuestion {index}: {question['question']}")
            if 'choices' in question:
                for choice in question['choices']:
                    print(choice)
        
        # Ask user for answer
            user_answer = input("Your answer: ").strip().capitalize()

        # Check if the answer is correct
            if user_answer == question['answer'].capitalize():
                print("Correct!")
                score += 1
            else:
                print("Incorrect.")

        # Display final score
            print("\nQuiz complete!")
            print(f"You got {score} out of {len(questions)} questions correct.")
    
    if __name__ == "__main__":
            run_quiz()

