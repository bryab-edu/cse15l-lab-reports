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
  public void testReversed() {
    int[] input1 = { };
    assertArrayEquals(new int[]{ }, ArrayExamples.reversed(input1));
  }
```
