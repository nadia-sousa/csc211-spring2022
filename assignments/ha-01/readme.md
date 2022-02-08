## Homework Assignment 01 (Due Date 02/5)

 This assignment is to be completed individually. You are not allowed to share your code with other students. The assignment is worth a total of 100 points. If you have any questions or need any help, please visit us during office hours and/or post questions on Piazza.

> If you need to post any of your actual source code on Piazza for any reason, **please** be sure to tag the post as being _visible to instructors only_, so that you don't inadvertently share code with others and violate class rules.

### Format details
Your submission will be tested and graded by an autograder, for this reason it cannot be stressed enough that your program must exactly follow the specifications for input and output upon submission.

If the question specifies that it will take a `double` then a `char` you must follow this input order or else fail the test.  For this assignment, you should use the `int` data type for regular whole numbers and as the default when a number format is not specified, you should use the `double` data type for any question which specifies decimal or floating point numbers, and `char` for single letter variables or input.

For details on expected submission instructions, please refer to the **Submission and Grading** section at the bottom of the document.

Before getting started, be advised that most of the questions will only require `std::cin` for reading the data (especially integers and floats).  If you need to read an arbitrary number of integers you can use a pattern like this, which will keep reading values until the end of the input:
```c++
while (std::cin >> value) {
  // do something with value
}
```
If otherwise, you want to read entire strings that include whitespaces the recommended fucntion is `std::getline`.  See below an example:
```c++
std::string name;
std::cout << "What is your name?";
std::getline(std::cin, name);
std::cout << "Hello " << name << "!\n";
```

# Above Average
It is said that 90% of frosh expect to be above average in their class. You are to provide a reality check.

## Input
The first line of standard input contains an integer 1≤C≤50, the number of test cases. C data sets follow. Each data set begins with an integer, N, the number of people in the class (1≤N≤1000). N integers follow, separated by spaces or newlines, each giving the final grade (an integer between 0 and 100) of a student in the class.

## Output
For each case you are to output a line giving the percentage of students whose grade is above average, rounded to exactly 3 decimal places.

### Sample Input 1
```
5
5 50 50 70 80 100
7 100 95 90 80 70 60 50
3 70 90 80
3 70 90 81
9 100 99 98 97 96 95 94 93 91
```
### Sample Output 1
```
40.000%
57.143%
33.333%
66.667%
55.556%
```



# License To Launch

Birk has made a new shiny rocket and just received his licence from the Bluesky Global Order (BGO) to launch anytime within the next n days. He is, however, worried that the rocket will hit space junk on its way. In order minimize the risk of a collision, Birk has made a model of how many pieces of space junk there will be for each of the next n days. He decided that he will launch his rocket on the day with the least space junk, and if there are multiple days with the same amount of space junk he of course wants to send his rocket up as early as possible.

Can you help Birk find out how many days he has to wait until he sends up his rocket?

## Input
On the first line there is a single integer n (1≤n≤100000) the number of days for which the launch license is valid. On the second line follows n integers between 0 and 109 where the i’th integer is the amount of space junk on the i’th day. The first day is day i=0.

## Output
Output a single integer, the number of days Birk needs to wait before he launches his rocket.

### Sample Input 1	
```
5
3 4 1 7 2
```
### Sample Output 1

```
2
```



# Hissing Microphone

A known problem with some microphones is the “hissing s”. That is, sometimes the sound of the letter s is particularly pronounced; it stands out from the rest of the word in an unpleasant way.

Of particular annoyance are words that contain the letter s twice in a row. Words like amiss, kiss, mississippi and even hiss itself.

## Input
The input contains a single string on a single line. This string consists of only lowercase letters (no spaces) and has between 1 and 30 characters.

## Output
Output a single line. If the input string contains two consecutive occurrences of the letter s, then output hiss. Otherwise, output no hiss.

### Sample Input 1	
```
amiss
```
### Sample Output 1
```
hiss
```

### Sample Input 2
```
octopuses
```
### Sample Output 2
```
no hiss
```

### Sample Input 3
```
hiss
```
### Sample Output 3
```
hiss
```

# Dot Product

![image](https://github.com/mfaramarzi/Internship_Summer2021/blob/master/david/Generators/DotProduct/VectorImage_cropped.JPG)

Calculating a dot product is a common practice in video game and graphics programming. 
One useful application of the dot product is that it allows us to determine the angle between two vectors in space.


For this assignment, you will be calculating the length of two vectors, and then computing their normalized dot product and outputting if the angle between the vectors is acute, obtuse, or perpendicular.
If the dot product of two vectors is 0, it means they are perpendicular.  If their dot product is greater than 0, it means the angle between them is acute.  If their dot product is less than 0, it means they are obtuse.

The formula for calculating a dot product of two vectors (in 2d space) is x1 * x2 + y1 * y2.

Normalizing a vector means that you are changing the length of a vector to be 1 (a unit vector).  You do this by dividing each x, y component by the length of the vector.

i.e. (x/length, y/length)

The formula for calculating the length of a vector is the Pythagorean formula: sqrt(x * x + y * y).

## Input
The input will be 4 integers separated by whitespace.  They will contain the x, y positions of the vectors: x1 y1 x2 y2.

## Output
The output will be a string in the format: 
```
Length of v1: <length_v1> 
Length of v2: <length_v2>
Their normalized dot product is <dot_product> and they are <angle> 
  ```
  
where angle is one of "Perpendicular, Acute, Obtuse" and the lengths and dot products are rounded to a precision of 4.
#### Sample Input 1
```
0 1 1 0
```
#### Sample Output 1
```
Length of v1: 1.0000
Length of v2: 1.0000
Their normalized dot product is 0.0000 and they are Perpendicular
```


### Submission and Grading
You will submit a single _zip file_ named `pa1.zip` through Gradescope.  Your zip archive must contain your source files **only**.  For each of the problems, create a file called `main_<num>.cpp` where _num_ is the question number itself with no leading zeros. Ensure _all_ of your code resides within the `main()` function within that file.  All programs **must** compile and execute without warnings.  Your programs will be automatically graded.  For each of the questions you either pass the test cases (full points) or not (zero points).

>You must be reminded that students caught cheating or plagiarizing will receive `no credit`. Additional actions, including a failing grade in the class or referring the case for disciplinary action, may also be taken.
