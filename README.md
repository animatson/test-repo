# Testing gt.sh

 Aim of this script is to help in Alx task , to reduce repetition of writing same git 
 commands each time you are doing a new task.That is to say think about when you have a script which do some simple git activity automatically thats the idea.

## How it Works
  After finishing to answer a question Alx require you to push your solution to github ,now you can run this script and take care of you.
* What it does is it will run _git add ._ and _git commit -m ""_ all this automatically then you can push your work to github easily
* Thats what it does fir now but we are hoping to improve it much more in the future.
  
## Sample scripts
  ```
#!/bin/bash
check=$(ls -a | grep .git)
if [ $check = ".git" ]; then
    git add .
    echo "write a commit message \n"
    read cmt
    git commit -m "$cmt"
else
    echo "Create a Repository then run Again"
fi

```
