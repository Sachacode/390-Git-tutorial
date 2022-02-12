# Learn Github With These Easy Steps: Programmers Hate This

Github is an excellent tool for the purpose of coding a project. Like all tools, one must first be able to use it or else it is pointless. While it may seem intimidating at first, this .md file will give you everything you need to know to get cracking on that coding assignemnt due in 2 hours. This tutorial covers the basic commands for uploading files to a repository, stashes, branches, and merging.

## Basic Commands
The flow of working on a project with Github revolves around working with a ***local repository*** and a ***remote repository***. The ***local repository*** is the project and its files stored on your computer. The ***remote repository*** is the project stored on your Github. With four easy comands `git clone [url]`, `git add filename`, `git commit -m`, and `git push`. In this tutorial we have provided a basic prject to follow along with. If you so desire you can fork this repo with ***fork*** button in the top right corner to follow along.

Now it's clonning time. Clonning a repository is what creates the ***local repository*** from the original ***remote repository***. For this tutorial we will be expolring the use of the command because it is widley used in the ***real world*** and it makes you look smarter than you actually are. To clone a repo put `git clone [url]` into the command line. The url for a repo can be accessed on the clone button in a repository, click to copy then paste into terminal.
```
git clone [url]
```

Congradulations, now you have an operational ***local repository***. Go into the file and add some code to the Main.java file prodivded. 
Example:
```java
public class Main {
    public static void main(String[] args) {
        System.out.println("I hate java with a passion...");
        //Add another fun and engaging print statemnt
        System.out.println("But javascript is even worse");
    }
}
```
Although your work looks all nice and saved this is far from the truth. You must now stage the changes you have to the file, the first part of saving changes on the ***local repository***. The `git add filename` command accomplishes this simple task, the filename in this tutorial would be `Main.java`.
```
git add
```
The next step to comitting the staged changes in the ***local repository*** and is putting `git commit -m` into the command line.
```
git commit -m
```
The -m refers the required message that must be put on every commit, recommoned messages include progress notes, dates, and whatever line of code you have starting at for the past hour that has ruined your day. Now the files on your ***local repository*** are all up to date, but what about that pesky ***remote repository***. The final step is upoloading to Github, simply type `git push` and horray, the ***remote repository*** is now up-to-date.
```
git push
```

## Stashes:
Great, now you have mastered the technique of the Github workflow but there is still knowledge to be leanred. Hypothetically lets say that you want to add another piece of code to the project, but you do not want it to commit it to the repo but you still want it to be saved. Good, because you can use the `git stash` command to save code temporarily without doing a commit.
```
git stash
```

## Branches:
An advantage of Github is its ability to have different versions of your project ready to go. Say you wanted to take your project and solve a problem multiple different ways that would interfer with each other. You can create different branches to accomplish this. Bracnhes are children of a commit, which use the parent as starting point from which the changes unique to the branch are made. Advantages of branches include explore different paths to creating tools, allowing different people to work on differet parts of a project without messing with each other, or keeping a previous version thatg is safe from whever disater you have have caused that breaks your code to the point where you would have to otherwise start over from the beginning.

## Merging:
