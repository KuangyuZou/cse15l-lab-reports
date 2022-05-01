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


The first code results in an infinite loop because the code ends with the blank line. When we delete the blank line, then the loop will run successfully. 

The second code results in only the last link content be returned. The reason is that this code ends with the valid link, the first link in newtest-file.md is not a valid link, so the results will not include the content in the first brackets. 

The third code results in an infinite loop because the code ends with the invalid link which is the bracktes. The valid link is in the middle so our code will run into an infinite loop that have no result. 