# quiz-game-project
questions = [
    {
        "question": "What is the capital of India?",
        "options": ["A. colombo", "B. Gandhi nagar", "C. New delhi", "D. chennai"],
        "answer": "C"
    },
    {
        "question": "What is 5 + 2?",
        "options": ["A. 3", "B. 7", "C. 5", "D. 6"],
        "answer": "B"
    },
    {
        "question": "What is the largest river in our in world?",
        "options": ["A. amazon", "B. nile", "C. missippi", "D. rio grande"],
        "answer": "B"
    }
]

def run_quiz():
    score = 0
    for q in questions:
        print(q["question"])
        for option in q["options"]:
            print(option)
        answer = input("Please enter your answer (A, B, C, D): ").strip().upper()
        
        if answer == q["answer"]:
            print("Correct!")
            score += 1
        else:
            print(f"Wrong! The correct answer was {q['answer']}.")
        print()  # Print a newline for better readability
    
    print(f"You got {score} out of {len(questions)} correct!")
    print("_________code excuteded sucessfully!_______")

if __name__ == "__main__":
    run_quiz()
