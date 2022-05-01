# First Code Change
![Image](firstcodechange.png)
[newtest-file](https://kuangyuzou.github.io/markdown-parser/newtest-file.html)
![Image](firstcodechangeOutput.png)

# Second Code Change
![Image](secondcodechange.png)
[newtest-file](newtest-file.html)
![Image](secondcodechangeOutput.png)

# Third Code Change
![Image](thirdcodechange.png)
[test2-file](test2-file.html)
![Image](thirdcodechangeOutput.png)


The first code results in an infinite loop because the code ends with the blank line. When we delete the blank line, then the loop will run successfully. 

The second code results in only the last link content be returned. The reason is that this code ends with the valid link, the first link in newtest-file.md is not a valid link, so the results will not include the content in the first brackets. 

The third code results in an infinite loop because the code ends with the invalid link which is the bracktes. The valid link is in the middle so our code will run into an infinite loop that have no result. 