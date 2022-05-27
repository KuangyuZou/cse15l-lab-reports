# Link of own and reviewded Reposiotory
[Own Reposiotory](https://github.com/KuangyuZou/markdown-parser)

[Reviewed Reposiotory](https://github.com/MichaelYe48/markdown-parser)

# For Each Test Task
## 1.Using VSCode Preview,

the Snippet1 should has the result as [`google.com,google.com, ucsd.edu]
![Image](preview1.png)

the Snippet2 should has the result as [a.com,a.com(()), example.com]
![Image](preview2.png)

the Snippet3 should has the result as [https://www.twitter.com, https://sites.google.com/eng.ucsd.edu/cse-15l-spring-2022/schedule, https://cse.ucsd.edu/]
![Image](preview3.png)


## 2.Showing the Test Code

The screenshot below shows the test for Snippet1,2,3 in my own MarkdownTest.java
![Image](first.png)

The screenshot below shows the test for Snippet1,2,3 in the reviewed MarkdownTest.java.
![Image](second.png)

## 3.Test Output for my own repository and Explaning
1).The screenshot below shows the test outputs of Snippet1.md by my own implemention of MarkdownParse.java.

![Image](ownoutput1.png)
From the result, the test for Snippet1 is failed. The actual result includes the "url.com" in the list besides other links. However, from the preview, we know that the "url.com" is an invalid link since the beginning of the this link is violated the correct link format in Markdown documents. This link begins with backtick instead of the bracket. My code does not verify that this link is an invalid link so it returns this link as well. I think the code change will small than 10 lines since we can just add an extra if statement to verify whether the beginning of the link format is correct so that the code can pass this test. 

2). The screenshot below shows the test outputs of Snippet2.md by my own implemention of MarkdownParse.java.
![Image](ownoutput2.png)
From the result, the test for Snippet2 is also failed. The actual result only return the "a.com" link. 


