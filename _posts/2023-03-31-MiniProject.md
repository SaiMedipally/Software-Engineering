I've been learning python as learning language, So we did mini-project based on python  named ```Typing_Tester```.

Python function called ```typing_test()```
that tests the user's typing accuracy and speed. 


The function imports the time module and a custom module generate_text that generates random text for the user to type.
The function starts by generating a random text using the ```generate_text()``` function and prints it out with instructions for the user 
to type the text as quickly and accurately as possible. It then waits for the user to press the ```Enter key before starting the test.```

The ```time.time()``` function is used to record the start and end times of the user's typing. The elapsed time is calculated by subtracting the start 
time from the end time.

The user's input is then compared to the generated text character by character. If the user input is shorter than the generated text, the function 
counts the remaining characters as errors. If the user input matches the generated text, no errors are counted. If the user input does not match 
the generated text, each incorrect character is counted as an error.

The function calculates the typing accuracy by subtracting the number of errors from the length of the generated text and dividing the result by
the length of the generated text. This value is then multiplied by 100 and rounded to the nearest whole number.

The typing speed is calculated by dividing the length of the generated text by the elapsed time and multiplying the result by 60 to convert from 
seconds to minutes. This value is also rounded to the nearest whole number.

Finally, the function prints out the user's input, the elapsed time, the typing accuracy, and the typing speed in words per minute (WPM).

***Skills/knowledge that I had learned earlier in the semester were useful in this project were:***


The ability to write code in Python and use built-in functions and modules like time is essential for this project.

Understanding how to generate random text using Python is required to create the ```generate_text()``` function.

Learned to prompt the user for input and display output using Python's ```built-in input()``` and ```print()``` functions is necessary.

Being able to manipulate strings and compare characters in Python is essential for calculating the user's accuracy and errors.


***The biggest challenge I faced during mini-project***


The biggest challenge in this mini-project algorithm to analyze the user's typing accuracy and to handle errors more effectively.

