To move forward with our recruiting process, we will need you to complete the task below.
The task is to write a simple application (any JAVA framework and version) which reads two parameters from the command line (java AppName firstParameter secondParameter). 
The first parameter defines an array containing values: 0 or 1 (for example 0100111010).
The second parameter is the number of iterations.
For the first iteration, the input array comes from the console command line.
For each next iteration, the input is the result of the previous iteration.
The application should implement an algorithm which goes through the array and changes values according to the following rules:
1. If the sum of adjacent neighbors is 0 or 2, the new value should be 0 (for example for 010 the next value of the second element will be 0).
2. If the sum of adjacent neighbors is 1, the new value should be 1.(for example for 011 the next value of the second element will be 1).
3. In case of the first and the last elements, take the only neighbor and apply rule 1 and 2.
Each element in an iteration is calculated based on the values from the input array.
Example:
java TestApp 01101 3
In each iteration the algorithm goes through all the elements:
1st element has only one neighbor which is 1 so the value will be 1
2nd element has two neighbors, 0 and 1, the sum is 1 so value will be 1
3rd element has two neighbors, 1 and 0, the sum is 1 so value will be 1
4th element has two neighbors, 1 and 1, the sum is 2 so value will be 0
5th element has only one neighbor which is 0 so the value will be 0
After the 1st iteration:   11100
After the 2nd iteration:   10110
After the 3rd iteration:   00111

The console app should validate the input parameters (check if the array and the number of iterations are correct).
The code should contain unit tests for the algorithm and input validation.
Your program will be automatically and manually tested.
