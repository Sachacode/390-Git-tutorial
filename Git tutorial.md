# Github Tutorial

Github is an excellent tool for the purpose of coding a project. While it may seem intimidating at first, this .md file will give you everything you need to know about the basics of Github. This tutorial covers the basic commands for uploading files to a repository, branches, stashes, and merging.

## Basic Commands
The flow of working on a project with Github revolves around working with a ***local repository*** and a ***remote repository***. The ***local repository*** is the project and its files stored on your computer. The ***remote repository*** is the project stored on your Github. With four easy commands `git clone [url]`, `git add filename`, `git commit -m`, and `git push`. In this tutorial we have provided a basic project to follow along with. If you so desire you can fork this repo with ***fork*** button in the top right corner to follow along.

Now it's time to clone the repository. Cloning a repository is what creates the ***local repository*** from the original ***remote repository***. For this tutorial we will be exploring the use of the command because it is widely used in the ***real world*** and it makes you look smarter than you actually are. To clone a repo put `git clone [url]` into the command line. The url for a repo can be accessed on the clone button in a repository, click to copy then paste into terminal.
```
git clone [url]
```

Congratulations, now you have an operational ***local repository***. Go into the file and add some code to the Main.java file provided. 
Example:
```java
public class Main {
    public static void main(String[] args) {
        System.out.println("I hate java with a passion...");
        //Add another fun and engaging print statement
        System.out.println("But javascript is even worse");
    }
}
```
Although your work looks all nice and saved, the changes have not been saved. You must now stage the changes you have to the file, the first part of saving changes on the ***local repository***. The `git add <filename>` command accomplishes this simple task, the filename in this tutorial would be `Main.java`.
```
git add <filename>
```
The next step to committing the staged changes in the ***local repository*** and is putting `git commit -m` into the command line.
```
git commit -m
```
The -m refers to the required message that must be put on every commit, recommoned messages include progress notes, dates, and whatever you want. Now the files on your ***local repository*** are all up to date, but what about that ***remote repository***. The final step is uploading to Github, simply type `git push` and now the ***remote repository*** is up-to-date.
```
git push
```
## Branches
An advantage of Github is its ability to have different versions of your project ready to go. Say you wanted to take your project and solve a problem multiple different ways that would interfere with each other. You can create a ***branch*** to accomplish this. ***Branches*** are children of a commit, which use the parent as starting point from which the changes unique to the branch are made. Advantages of ***branches*** include explore different paths to creating tools, allowing different people to work on different parts of a project without messing with each other, or keeping a previous version that is stable. You can type `git branch <branchname>` to create a ***branch*** with a name.
```
git branch <branchname>
```
To delete a ***branch*** type `git branch -d <branchname>`.
```
git branch -d <branchname>
```
## Stashes
Great, now you have mastered ***branches*** but there is still more to know. Hypothetically let's say that you want to add another piece of code to the project, but you do not want it to commit it to the repo but you still want it to be saved. Good, because you can use the `git stash` command to save code temporarily without doing a commit. This creates a ***stash***, which is a temporary ***branch*** that is a snapshot of current changes that have not been committed yet.
```
git stash
```
To save changes in a ***stash*** use the `git stash pop` command.
```
git stash pop
```
## Merging
***Branches*** are great but what if you want to combine changes in your ***branch*** back to the main, you can do a ***merge***. All you need to do is use `git merge <branchname>` and the ***branch*** will be ***merged*** into the main.
```
git merge <branchname>
```
This will work great if you have one ***branch*** being ***merged***, but problems may occur if you have two ***branches*** with conflicting code. You will need to clean up your code to make sure that nothing is conflicting to complete the ***merge***. For example if you have two ***branches*** with a variable added to Main.java with slightly different code you have a conflict if you try to ***merge*** into main.

Branch A:
```java
public class Main {
    public static void main(String[] args) {
        System.out.println("I hate java with a passion...");
        //Add another fun and engaging print statement
        System.out.println("But javascript is even worse");
        
        //check out my awesome variable
        int x = 1;
    }
}
```
Branch B:
```java
public class Main {
    public static void main(String[] args) {
        System.out.println("I hate java with a passion...");
        //Add another fun and engaging print statement
        System.out.println("But javascript is even worse");
        
        //check out my awesome variable
        int x = 0;
    }
}
```

## Conclusion
Now you should have the basics ready to go for using Github for your coding career. It is a powerful and widely used tool that is essential for programming these days, and after getting the hang of Github, you will be a pro in no time.
