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
