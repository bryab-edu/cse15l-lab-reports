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

## Part 2 - Researching Commands `find`
### The `find -size` command option [source](https://man7.org/linux/man-pages/man1/find.1.html)
Example 1 <br>
```
$ find -size +200k
./911report/chapter-13.4.txt
./911report/chapter-13.5.txt
./911report/chapter-3.txt
./government/About_LSC/commission_report.txt
./government/Env_Prot_Agen/bill.txt
./government/Gen_Account_Office/d01591sp.txt
./government/Gen_Account_Office/GovernmentAuditingStandards_yb2002ed.txt
./government/Gen_Account_Office/pe1019.txt
./government/Gen_Account_Office/Statements_Feb28-1997_volume.txt
```
Can search for files within working directory greater than the inputed requirements (+200k means files greater than 200 kilobytes). Good for finding which files take up most of the memory (e.g when downloading a repository) <br> <br>
Example 2 <br>
```
$ find 911report/ -size -50k
911report/
911report/chapter-10.txt
911report/preface.txt
```
Can search for files within a specific directory less than the inputed requirements (-10k means files less than 10 kilobytes). Good for filtering out specific files within a memory range.
### The `find -readable` command option [source](https://man7.org/linux/man-pages/man1/find.1.html)
Example 1 <br>
```
$ find 911report/ -readable
911report/
911report/chapter-1.txt
911report/chapter-10.txt
911report/chapter-11.txt
911report/chapter-12.txt
911report/chapter-13.1.txt
911report/chapter-13.2.txt
911report/chapter-13.3.txt
911report/chapter-13.4.txt
911report/chapter-13.5.txt
911report/chapter-2.txt
911report/chapter-3.txt
911report/chapter-5.txt
911report/chapter-6.txt
911report/chapter-7.txt
911report/chapter-8.txt
911report/chapter-9.txt
911report/preface.txt
```
Can search for files marked readable permissions to the current user in a specific directory. Good for filtering out files that can be read by the user. (i.e allowed permission files) <br> <br>
Example 2 <br>
```
$ find -readable
./911report/...
./biomed/...
./government/...
./plos/...
```
^ given the circumstances, this essentially printed all directories and files in the `pwd` <br>
Can search for files marked readable permissions to the current user in the current directory.

### The `find -name` command option [source](https://man7.org/linux/man-pages/man1/find.1.html)
Example 1:
```
$ find -type d -name "biomed"
./biomed
```
Can search (and is useful for trying to find) the inputted directory given the name in the current direcotry (type d for directory). <br> <br>
Example 2:
```
$ find -name chapter-1.txt
./911report/chapter-1.txt
```
Can search (and is useful for trying to find) the inputted file given the name in the current directory. (also given the extension) <br> <br>

### The `find -anewer` command option [source](https://man7.org/linux/man-pages/man1/find.1.html)
Example 1:
```
$ find -anewer 911report/chapter-2.txt
./plos/pmed.0020145.txt
./plos/pmed.0020146.txt
./plos/pmed.0020148.txt
./plos/pmed.0020149.txt
./plos/pmed.0020150.txt
./plos/pmed.0020155.txt
./plos/pmed.0020157.txt
./plos/pmed.0020158.txt
./plos/pmed.0020160.txt
./plos/pmed.0020161.txt
./plos/pmed.0020162.txt
```
^ this is a portion size of the output, includes files from other directories within `technical/` as well <br>
Can search for files that have been accessed more recently than the the provided file. Good for measuring updates (outdated files, patches) of an apps contents <br> <br>
Example 2:
```
$ find -anewer biomed/
./plos/pmed.0020232.txt
./plos/pmed.0020235.txt
./plos/pmed.0020236.txt
./plos/pmed.0020237.txt
./plos/pmed.0020238.txt
./plos/pmed.0020239.txt
./plos/pmed.0020242.txt
./plos/pmed.0020246.txt
./plos/pmed.0020247.txt
./plos/pmed.0020249.txt
./plos/pmed.0020257.txt
./plos/pmed.0020258.txt
./plos/pmed.0020268.txt
./plos/pmed.0020272.txt
./plos/pmed.0020273.txt
./plos/pmed.0020274.txt
```
^ sample size again <br> <br>
Can search for files that have been accessed more recently than the provided directory. More general means of date comparison


