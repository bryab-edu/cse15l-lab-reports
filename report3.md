# Lab Report 3 - Bugs and Commands
## Part 1 - Bugs
### Bug Input - Arrays with length greater than 1
```
@Test
  public void testReversedFilled(){ 
    int[] input2 = {1, 2, 3};
    int[] input2_reversed = {3, 2, 1};
    assertArrayEquals(input2_reversed, ArrayExamples.reversed(input2));    Expected [3] but was [0]
  }
```
### Passing Input - Arrays with lengths less than or equal to 1
```
@Test 
	public void testReverseInPlace() {
    int[] input1 = { 3 };
    ArrayExamples.reverseInPlace(input1);
    assertArrayEquals(new int[]{ 3 }, input1);
	}


  @Test
  public void testReversed() {  <=== We'll focus on this one
    int[] input1 = { };
    assertArrayEquals(new int[]{ }, ArrayExamples.reversed(input1));
  }
```
### JUnit Tests testReversed()
#### ![Image](https://bryab-edu.github.io/cse15l-lab-reports/report3files/codeShot1.PNG)
### The Code Bug in testReversed() method
#### Original Code
#### ![Image](https://bryab-edu.github.io/cse15l-lab-reports/report3files/codeShot2.PNG)
The bug of the method is it incorrectly copies values from the new empty array (which are all 0) onto the parameter array. Therefore, the array's values would all be replaced by 0.
#### Fixed Code
#### ![Image](https://bryab-edu.github.io/cse15l-lab-reports/report3files/codeShot3.PNG)
To fix this, we modify lines 17 and 19: <br>
Line 17: newArray[i] = arr[arr.length - 1 - i]; <== This accurately adds each element from the end of the array on to the newArray <br>
Line 19: return newArray; <== fixes the issue where despite creating a whole different array, the unchanged input array is returned
#### Passed Tests
#### ![Image](https://bryab-edu.github.io/cse15l-lab-reports/report3files/codeShot4.PNG)



