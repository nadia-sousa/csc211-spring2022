## Mini Programming Challenge #02 (Due Date 02/13)

This mini-challenge is about getting you comfortable with the autograder and basic C++ arethmatic operations. **Arrays, functions, and loops are not allowed. The only libraries allowed for this assignment are `<iostream>` and `<iomanip>`**.  Mini-challenge problemsets are to be completed individually. You are not allowed to share your code with other students. The assignment is worth a total of 100 points. If you have any questions or need any help, please visit us during office hours and/or post questions on Piazza.

> If you need to post any of your actual source code on Piazza for any reason, **please** be sure to tag the post as being _visible to instructors only_, so that you don't inadvertently share code with others and violate class rules.

### Format details
Your submission will be tested and graded by an autograder, for this reason it cannot be stressed enough that your program must exactly follow the specifications for input and output upon submission.

If the question specifies that it will take a `double` then a `char` you must follow this input order or else fail the test.  For this assignment, you should use the `int` data type for regular whole numbers and as the default when a number format is not specified, you should use the `double` data type for any question which specifies decimal or floating point numbers, and `char` for single letter variables or input.

The output will always be some form of string printed out on a single line. It will always begin on a new line and end with some form of newline character; either `std::endl` or `'\n'`.  Whenever printing a `double` you should always have exactly 4 decimal places; if your decimal number is `3.1415926534`, you should print it as `3.1416`. If your number is `0.0` or `0`, it should print as `0.0000`. You can use `<iomanip>` to accomplish this.

For details on expected submission instructions, please refer to the **Submission and Grading** section at the bottom of the document.

1.  *Odd or even*. Sometimes it will be useful to know whether a given number is odd or even. This program should read a single integer number from the user and print whether or not the provided number is even or odd. The output should be a single line formatted as follows: `<number> is <odd|even>` where `number` is replaced by the user input, and `odd` or `even` is printed depending on whether or not the number is odd or even.  You are encouraged to use the ternary operator to complete this program.

2. *Last digit is 9*. Prompt the user for an integer number. If the last digit of the entered number is 9, print `<number> is good`, otherwise, print `<number> is no good`. Some examples of "good" numbers would be: 9, 19, 1279, 999, 699, 1029 etc.

3. *Average*. Prompt the user for three decimal values and print the average of the three in the format: `The average of <num1>, <num2>, and <num3> is <average>`.

4. *Positive or negative*. This program should prompt the user for an integer number and print whether the provided number is positive or negative. The output should be a single line formatted as follows: `<number> is <positive|negative>`.  If the number is zero, the output string should instead print `<number> is neither positive nor negative`.


### Submission and Grading
You will submit a single _zip file_ named `mc2.zip` through Gradescope.  Your zip archive must contain your source files **only**.  For each of the problems, create a file called `main_<num>.cpp` where _num_ is the question number itself with no leading zeros. Ensure _all_ of your code resides within the `main()` function within that file.  All programs **must** compile and execute without warnings.  Your programs will be automatically graded.  For each of the questions you either pass the test cases (full points) or not (zero points).

>You must be reminded that students caught cheating or plagiarizing will receive `no credit`. Additional actions, including a failing grade in the class or referring the case for disciplinary action, may also be taken.
