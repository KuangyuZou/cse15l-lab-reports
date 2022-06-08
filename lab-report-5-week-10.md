# Different Tests using Vimdiff
![Image](difftest1.png)
![Image](difftest2.png)
![Image](difftest3.png)
I use vimdiff command and the output redirection to see the difference tests result between my repository and the given repository. 

# Test-file Link
[test-files](https://github.com/nidhidhamnani/markdown-parser/tree/main/test-files)

# Chosen  Two Tests out of 652 overall tests.
For the two tests, I choose the 508.md file and the 487.md file. 

# Each Test Explaination
## 1. My Own Repository test result.
1) For the 508.md file test, my implementation is correct. Since from the preview in VSCode,
![Image](508.png)
we know that this link is valid and the expected output should be[/url 'title "and" title']. My actual output is the below picture from vimdiff results.txt:
![Image](508_own.png)

2. For the 487.md file test, my implementation is incorrect. Since from the preview in VSCode,
![Image](487.png)
We know that this linke is not valid, so the expected output should be [ ].
My actual is the below picture showing:
![Image](487_own.png)

## 2. The Given Repository test result.
1. For the 508.md file test, the given implementation is incorrect. Since from the preview in VSCode as indicated above, the expected output should be[/url 'title "and" title']. However, the actual output is below screenshot showing:
![Image](508_given.png)



2. For the 487.md file test, the given implementation is correct. Since from the preview in VSCode as indicated above, the expected output should be[ ].
The actual output from the given repository is the below screenshot showing:
![Image](487_given.png)

# Wrong Output Explaination
1. For the 508.md test file, my implemention is correct but the given implemention is wrong. The given implemention returns nothing which is an empty list. The reason is that, from the code below:
![Image](given_code.png)
