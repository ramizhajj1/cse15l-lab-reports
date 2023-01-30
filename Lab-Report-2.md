# Lab Report 2  

In this lab report, we will cover topics such as symptoms, failure inducing imputs, and web server creation.   

## Symptoms and Failure Inducing Input  

Symptoms and failure inducing input are two very important concepts when it comes to testing and assuring the quality of code. By using failure inducing imput, bugs can be found easily in code and fixed.   

In our labs, we used JUnit tests to test if our code was returning the correct output for our implemented input.   

We began with a buggy piece of code, and in order to find the bug, we implemented an example of failure inducing input in the following code:   

```
# code block
public class ArrayTests {
	@Test 
	public void testReverseInPlace() {
    int[] input1 = { 3, 4, 5 };
    ArrayExamples.reverseInPlace(input1);
    assertArrayEquals(new int[]{ 5, 4, 3 }, input1);
	}
```
  
The failure inducing input was that by using {3,4,5} when the array was not changed, for reversed the new array is empty, and so all elements are 0. The bug was that the initial output was {0,0,0} because the array was empty because we were assigning the array elements to an empty array.   

The corresponding input for the symptom in testReverseInPlace was [5, 4, 5] instead of [5,4,3].  

As you can see in the following code, the JUnit test is failed because the expected output of the array is not what the function returns, hence the bug.  

Because the array is empty at reversed, if you put in an expected output of [0,0,0], you will see that is passes the JUnit test in the image below.   


