## Q1 : Sometimes many developers committed the code to the project and then they realize that code they committed is the wrong one. 

## Give 2 git command to reset to specific commit id and give the explain how it different? 


    git reset --soft <commit id>


    - This reset type changes you into the staging area and then you can make one big commit right afterward.


    get reset <commit id>


    - This reset move those changes back to the working directory if you've made some commits and you still want it to be in history that you want to regroup the way those commits are made.


href : https://git-scm.com/docs/git-reset

href: https://www.youtube.com/watch?v=Yho1Fs-gR9s



## Q2 : Sometimes developer writing code and see the warning sign that ide tell but they ignore it because they running it and it works fine not have any problems. 

## What is the pad that suitable it and write some code it has the warning sign and describes how it can affect you program?



### - PAD No.34 Treat warning as error



### Example code in c++ (uninitialized variable):

    #include <cstdio>

    int main() {

    bool text;

    if (text) { puts("Polls"); }

    if (!text) { puts("Result"); }

    }

     Output : Goodbye


### A2 : Think that the value of text is either be true or false,so "Polls" or "Result" is printed but in these case it print only "Result". 


href: https://mortoray.com/2014/04/16/the-uninitialized-variable-anathema-non-deterministic-c/


## Q3 : In the projects when developers working code by don't consider the order by the important task then it make your project didn't on time,
## What is the best habits to fixing it and how to fix this? 


#### A3:
## - Habit 3 - Put First Things First
## - You must apply effort to the most important task first, followed by a less important task.



href: https://simpleprogrammer.com/7-habits-highly-effective-programmers/


## Q4 : Why retrospective is important for scrum framework?

#### A4:
    [x] Boost team spirit
    [ ] Provide the platform for scrum team
    [x] Discover risks early
    [ ] Find mistake task
    [x] Create transparency and trust

href : https://wunder.io/


## Q5 : When many developers working in same repository projects they work separately and when they finish their work, They push the change file to the repository then they have many of conflict in the code that makes them lost their time to continue working.

## What is the best way to avoid this situation?


 #### A5:
- They should use git flow to avoid the conflict by creating 3 different branches

  - Feature branch uses to develop a new feature and then when it did we merge it into the develop branch.

  - Release branch it a copy of develop to be deployed, the task in this branch is to fix bugs and make some document.

  - Hotfix branch it copy of master sometime call maintenance branch,task in this branch to fix critical bugs.

href : https://www.algorithmtut.com/git-flow-and-code-review/