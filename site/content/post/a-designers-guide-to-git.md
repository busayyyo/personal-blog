---
title: A designer's guide to git
date: 2020-01-16T03:03:47.054Z
description: test
---
There have been so many debates on whether a designer should learn how to code - this is not one of them. However, there are many times within a team, that a designer may be required to provide developers assets they need or maybe even write a snippet of CSS. As digital teams get more diverse and roles overlap, working collaboratively becomes essential. One tool that makes this collaborative experience run smoothly is git. Learning how to use git efficiently can be a distinctive skill that will improve your efficiency and relationships with the developers on your team. And you don't even even need to know everything about git to get to this level of efficiency.

## A little note on git

Git is a version control system that basically keep tracks of all the changes in your file. It helps you write code safely knowing you can keep track of changes and even undo them in the event of a code mishap. Imagine if you didn't have Ctrl-Z, how horrible would writing a text file be. But unlike most text document management tool, Git keep tracks of all the timeline of your writing as long as you commit. If there's any takeaway you get from this article let it be this - Remember to commit your changes! But let's get cracking of what a likely scenario of using git can look like for a designer. Github hosts repository, basically code bases that utilise git.

## A likely scenario

Imagine there's a part of your company's web app you've recently redesigned to improve usability. It's an important change, something that will save the customer support people a few calls, but the developers are busy with the sprint and can't spare the time. You on the other hand, can manage the change since you are a CSS guru and a designer who knows the implication of the change not going out with the next release. You get a go ahead from the product and engineering managers, who say go make the change. How do you make these changes and work collaboratively with your teammates without messing things up for anyone involved?

Here's how:

**0. Check branch:** Shows you the current branch

`git branch`

**1. Pull:** The first thing you want to do is get the current state of the web app into your local computer. 

`git pull remote`

**2. Branch:** You want to create a branch for it. Think of it like creating your own playground, where if you mess up, it's only your own mess and you have time to clean it up. Branching is essential to working collaboratively with git. You have to remember to do  this.

`git branch playground`

**3. Status:** You can check the status of your branch by typing git status. Status shows you the files that have been changed but not yet committed.

`git status`

**4. Add:** After you must have made the changes in a file, you can add it. Adding makes the git begin to track the changes you make to that file.

`git add <filename>`

**5. Commit:** Commit is making git aware of your changes

`git commit -m "adds instruction snippet to web page"`

**6. Log:** Shows you the history of all commits in the current branch

`git log`

**7. Merge:** Merge your branch with the main one.

`git merge instruction snippet`

**8. Push:** Makes your code live with the repository.

`git push origin master`

## Conclusion

This is by no means the end to git. But this is likely to be your most typical workflow when working with git as a designer. Pull, branch, status, add, commit, merge, push - understanding these 7 commands will help you work effectively. But just incase it all seems so tedious with the command line interface, you can also use apps such as the GitHub desktop app if your team's repository is hosted on Github.
