Experiment – 7
Title 1: Study of For Loop and While Loop in Python
Aim

To study and implement the use of for loop and while loop in Python programming.

Theory

Looping is a control structure that allows a set of statements to be executed repeatedly based on a condition or over a sequence. Python provides two main types of loops:

for loop

while loop

 Algorithm 1: Using For Loop to Print Numbers from 1 to 5

Start

Use range(1,6) to generate numbers from 1 to 5

Assign each value to variable i one by one

Print the value of i

Stop

Program
for i in range(1, 6):
    print(i)

Output
1
2
3
4
5

 Algorithm 2: Using While Loop to Print Numbers from 1 to 5

Start

Initialize variable i = 1

Check condition i <= 5

If true, print i

Increment i by 1

Repeat steps 3–5 until condition becomes false

Stop

Program
i = 1
while i <= 5:
    print(i)
    i += 1

Output
1
2
3
4
5

Difference Between For Loop and While Loop

for loop is used when number of iterations is known.

while loop is used when number of iterations depends on a condition.

for loop automatically manages iteration.

while loop requires manual updating of variable.

Title 2: Study of While Loop with Break, Continue and Pass Statements
Aim

To study and implement break, continue, and pass statements in a while loop.

 Algorithm 3: Using Break in While Loop

Start

Initialize i = 1

Repeat while i <= 10

If i == 8, terminate loop using break

Otherwise print i

Increment i

Stop

 Algorithm 4: Using Continue and Pass in While Loop

Start

Initialize i = 1

Repeat while i <= 10

If i == 3, execute pass

If i == 5, increment i and skip iteration using continue

If i == 8, terminate loop using break

Print i

Increment i

Stop

Program
i = 1
while i <= 10:

    if i == 3:
        pass

    if i == 5:
        i += 1
        continue

    if i == 8:
        break

    print(i)
    i += 1

Output
1
2
3
4
6
7

Title 3: Study of For Loop with Break, Continue and Pass Statements
Aim

To study and implement break, continue, and pass statements in a for loop.

 Algorithm 5: Using Break, Continue and Pass in For Loop

Start

Use range(1,11) to generate numbers 1 to 10

For each value of i

If i == 3, execute pass

If i == 5, skip iteration using continue

If i == 8, terminate loop using break

Print i

Stop

Program
for i in range(1, 11):

    if i == 3:
        pass

    if i == 5:
        continue

    if i == 8:
        break

    print(i)

Output
1
2
3
4
6
7

Conclusion

Thus, the for loop and while loop were studied and implemented successfully using Python programs.
The working of break, continue, and pass statements in both loops was also studied and understood.
