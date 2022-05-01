# First Code Change
![Image](firstcodechange.png)
[newtest-file](https://kuangyuzou.github.io/markdown-parser/newtest-file.html)
![Image](firstcodechangeOutput.png)
After fix the code, the picture below shows that the code pass the test and also the origial testfile can also be passed.
![Image](fixcodepasstest1.png)

# Second Code Change
![Image](secondcodechange.png)
[test2-file](https://kuangyuzou.github.io/markdown-parser/test2-file.html)
![Image](secondcodechangeOutput.png)
After fix the code, the picture below shows that the code pass the test and also the origial two testfiles also passed.
![Image](fixcodepasstest2.png)

# Third Code Change
![Image](thirdcodechange.png)
[test3-file](https://kuangyuzou.github.io/markdown-parser/test3-file.html)
![Image](thirdcodechangeOutput.png)
After fix the code, the picture below shows that the code has a correct output which will not return the string in the parentheses sice this is the image refrence.
![Image](fixcodechangetest3.png)


The first code results in an index out of bound problem because there is no link in the newtest file, so the code does not find the opened parenthese and the closed parenthese. Therefore, there is no substring between the parentheses since no parentheses found. So the code will have index out of bound problem when call the method "markdown.substring(Openparen+1, closeParen)", the screenshot of output indicates "it begins at 0, but ends with -1". So if we want to fix the bug, we just need to add a condition at the front when the index of OpenParen is 0, then the code should break and return an empty list. 

The second code results in an infinite loop because the link is at the start of the test2 file, so the currentindex will always less than the markdown length. Therefore, in the while condition statement, since the currentIndex will always less than the markdown length, the while loop will infite. If we want to fix the bug, we just need to add another condition at the front which is when the Openbracket index is 0, then the code should directly return the string in the link, instead of increase the currentIndex value.

The third code results in a wrong output since this is actually an image refrence not the link. So we need to change code to verify whether the refrence is a link or an Image. So we need to add another condition at front which is when the string in the bracket is "Image", then the code should verify that this is not a link and should break and return an empty list. 