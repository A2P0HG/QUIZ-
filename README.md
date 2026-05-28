Markdown

This project is a beginner-level Python Quiz Application made using basic Python programming concepts. The quiz asks users multiple questions, takes answers as input, checks whether the answers are correct or wrong, and displays the final score at the end.
The project also includes a timer feature that measures how much time the user takes to answer each question. If the user gives a wrong answer, the app provides a helpful hint and gives a second chance to answer correctly. This makes the quiz more interactive and user-friendly.
The project uses important Python concepts such as:
Variables
Input and Output
Conditional Statements (if, elif, else)
Time Module
String Functions (lower())
Score Counter
Nested Conditions
Features of the Quiz App:
Multiple quiz questions
Timer for each question
Hint system
Retry/second chance feature
Final score display
User-friendly interaction
This project is useful for Python beginners to practice logic building and understand how real quiz applications work.
# Quiz App
import time

score = 0

# Question 1
question1 = "Which is the national bird of India?"
correct_answer1 = "peacock"

print("\nQuestion 1")
print(question1)

start_time = time.time()

answer = input("Your answer: ")

end_time = time.time()

time_taken = end_time - start_time

print("You took", round(time_taken, 2), "seconds")

if time_taken > 10:
    print("Time up!")

elif answer.lower() == correct_answer1:
    print("Correct!")
    score += 1

else:
    print("Wrong!")
    print("Hint: It is famous for colourful feathers.")

    answer = input("Try again: ")

    if answer.lower() == correct_answer1:
        print("Correct!")
        score += 1

    else:
        print("Wrong again!")
        print("Correct answer is:", correct_answer1)

# Question 2
question2 = "What is the name of Prime Minister of India?"
correct_answer2 = "narendra modi"

print("\nQuestion 2")
print(question2)

start_time = time.time()

answer = input("Your answer: ")

end_time = time.time()

time_taken = end_time - start_time

print("You took", round(time_taken, 2), "seconds")

if time_taken > 20:
    print("Time up!")

elif answer.lower() == correct_answer2:
    print("Correct!")
    score += 1

else:
    print("Wrong!")
    print("Hint: He became Prime Minister in 2014.")

    answer = input("Try again: ")

    if answer.lower() == correct_answer2:
        print("Correct!")
        score += 1

    else:
        print("Wrong again!")
        print("Correct answer is:", correct_answer2)

# Final Result
print("\nQuiz Finished!")
print("Final Score:", score)