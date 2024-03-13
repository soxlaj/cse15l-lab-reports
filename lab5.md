## Part 1

**Student Post:**

```
Hi, I’ve had trouble understanding why my output is incorrect for my tests on Filter1 where I’m not sure why the expected appears like that given I used the same kind of formatting for merge and the expected also looks a little weird where it seems to be a reference to an array, but it seems to have worked for merge so I’m confused as to why filter won’t run correctly since its expected should match the actual output since it appears to be an array that is returned.

```

**TA Response:**
```
Hi, it appears that your code expects an array of strings to be returned from your filter method but it returns an array however this is not in the return type of an array which is the difference between your merge and filter test where your filter is missing the “.toArray” that your merge tests contain, this may be the reason for the bug/issue you’re experiencing however without an insight into your actual code for your method I cannot express whether this is correct but you should fix your tests appropriately to maintain the same return type for the expected and actual output.
```

**Student Response:**
```
Hi! Thank you so much for your feedback, I tried what you suggested and it seems that it worked and it does appear there was a disparity between the return types and that the returned value from the filter method needed to be typecasted to an Array from an ArrayList because the test expected an array to be returned but instead compared against an ArrayList and therefore the test failed, but after fixing that the tests passed. However I did noticed that it started giving me lines such as “Note: ListExamplesTests.java uses or overrides a deprecated API.” and another line below so I wonder why that is.


```
**Setup**

```
1) Edited git clone of lab7 in the remote server of soxlaj@ieng6-202.ucsd.edu
cd into lab7
```
2) Screenshot of ListExamplesTests.java

3) `bash test.sh`

4) The actual output of both filter tests needed to be fixed to typecast into an Array where an ArrayList would throw an error since you can’t compare an array with an ArrayList. Where the outputs of the Strings would not match even though they contain the same elements. 


## Part 2
Something I learned in the second half of the quarter was the existence of `vim` and how that can connect with `git` and being able to do local commits and push it into the public and online version and how `vim`, as a text editor, helps in changing files that you can’t visually see. Mostly, `vim` can be useful to changing and updating files and even combining it with other commands to make changes to files which can be useful in circumstances where you are unable to access the files visually. It may not be the most efficient or easy method but I think it is really interesting that this old program remains in use and that we can continue to find use in it where we can simply just enter the mode no matter the file as long as we are in the right directory. 
