import time

score = 0

# Question 1
question1 = "Which is the national bird of India?"
correct_answer1 = "peacock"

print(question1)

start_time = time.time()

answer = input("Your answer: ")

end_time = time.time()

time_taken = end_time - start_time

print("You took", round(time_taken, 2), "seconds")

if time_taken > 10:
    print("Time up!")
elif answer.lower() == correct_answer1:
    print("Correct")
    score += 1
else:
    print("Wrong")
    print("Correct answer is:", correct_answer1)

print()


# Question 2
question2 = "What is the name of Prime Minister of India?"
correct_answer2 = "narendra modi"

print(question2)

start_time = time.time()

answer = input("Your answer: ")

end_time = time.time()

time_taken = end_time - start_time

print("You took", round(time_taken, 2), "seconds")

if time_taken > 20:
    print("Time up!")
elif answer.lower() == correct_answer2:
    print("Correct")
    score += 1
else:
    print("Wrong")
    print("Correct answer is:", correct_answer2)
print("quiz finished")

