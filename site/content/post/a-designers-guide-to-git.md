---
title: A designer's guide to git
date: 2020-01-16T03:03:47.054Z
description: >-
  Find yourself in a situation where you have to use git as a designer? Here's
  your guide:
---
![](/img/grayscale-photo-of-computer-laptop-near-white-notebook-and-169573.jpg)

There have been so many debates on whether a designer should learn how to code - this is not one of them. However, there are many times within a team, that a designer may be required to provide developers assets they need or maybe even write a snippet of CSS. As digital teams get more diverse and roles overlap, working collaboratively becomes essential. One tool that makes this collaborative experience run smoothly is git. Learning how to use git efficiently can be a distinctive skill that will improve your efficiency and relationships with the developers on your team. And you don't even even need to know everything about git to get to this level of efficiency.

## A little note on git

Git is a version control system that basically keep tracks of all the changes you or your teammates make to a file (in this case, your team's code repository). It helps you write code safely knowing you can keep track of changes and even undo them in the event of a code mishap. Imagine if you didn't have Ctrl-Z, how horrible would writing a text file be? But unlike most text document management tool, Git keep tracks of all the timeline of your writing as long as you commit. If there's any takeaway you get from this article let it be this - _Remember to always commit your changes!_ 

But let's see what a likely scenario where a designer may get to use git.

## A likely scenario

Imagine there's a part of your company's web app you've recently redesigned to improve usability. It's an important change, something that will save the customer support folks a few calls, but the developers are busy with the sprint and can't spare the time. You on the other hand, can manage the change since you are a CSS guru and a designer who knows the implication of the change not going out with the next release. You get a go ahead from the product and engineering managers, who say 'go make the change!' How do you make these changes and work collaboratively with your teammates without messing things up for anyone involved?

Here's how:

> **Note:**
>
>  For the purpose of this article, I have created a GitHub repository that you use in following along with this article: https://github.com/busayyyo/designers-guide-to-git

**1. Clone repository:** The first thing you wanna do is clone your team's remote repository. It will be on a code repository manager such as GitHub, Bitbucket or Gitlab. Cloning allows you to create a copy of the repository into your local machine. You clone using this command: `git clone <remote repository address>`

`git clone https://github.com/busayyyo/designers-guide-to-git`

**2. Check and maybe switch branch:** Now that you have the cloned files locally, the next step is to check where you are. Think of branches as rooms in your communal living repository house. You want to be in the right room before you decide to paint a wall red. 

To do this, first go into the house, i.e the directory where your cloned repository now is. You do this using the \`cd directory name\` command, in this case: `cd designers-guide-to-git`

Then use the command: `git branch # shows you the current repository, i.e room where you are right now`

Let's say you find yourself on the master branch... that's a room you don't wanna be in while you paint the town red. Get out of there and go to the branch your teammates develop on. We'll call that 'develop'.
`git checkout develop # switches you to the right room.`

**3. Pull:** Between cloning, branch switches and the bathroom break you just had, your teammates may have pushed new changes to the develop branch you are on. You want those changes in your local version as well and it's good practise to always pull them in every chance you get. To do that, all you have to do is: 

`git pull origin develop`

**4. Branch:** Now that you have the latest changes in the develop branch, you wanna get cracking, yeah? Well, not so fast. Remember, the develop branch is the communal room what everyone on your team pushes to, before going live. It may not be the master room but it is still sacrosanct and you don't wanna mess it up. You want to create your own branch. Think of it like creating your own playground, where if you mess up, it's only your own mess and you have time to clean it up. Branching is essential to working collaboratively with git. To create your own branch, use the command `git branch <branch-name>` as in:

`git branch playground`

Next thing to do is go into your playground that you just created using the command `git checkout <branch-name>` as in:
`git checkout playground`

This new branch is a copy of the branch develop, difference is, you can paint this playground red, if you wish.

**5. Status:** You can check the status of your branch by typing git status. Status shows you the files that have been changed but not yet committed.

`git status`

Since we have't made any concrete changes to the file just yet, you won't get much of a feedback regarding your files. This is time to give git a break, go into the CSS file you wanna make changes to and do your CSS magic.

**6. Add:** After making changes in a file, you should add it. Adding makes the git begin to track the changes you make to that file. You can can add all changes  `git add <filename> or git add .`

A little side note, the . after the add command stands for directory. So in essential, you are saying add all the changes in this directory.

**7. Commit:** Committing is very important. Committing is creating a record of the changes you have just added. You get a short SHA code after commit. This code can be used to roll back changes just in case you decide that was the wrong change or you wanna go back to a previous version. It is essential to add a commit message - which is a short description of the change you just made.

`git commit -m "changes button color to red"`

`It's good practise to commit changes as often as you can. You can break your commits into fixes. For example, if your tasks are comprised of 3 major fixes, it's best to commit after completing each one. That way, you can roll back changes`

**8. Log:** Logging is a useful practice for keeping track of your commits. It shows you the history of all commits in your current branch. Every now and then, you may want to see the log of all the commits you have made or your teammates made to the develop branch (yes, you will see that too, since your branch is a clone of the develop branch). To do that it's as simple as typing: 

`git log`

**9. Push:** Say you've made all the usability changes you want to and you've added and committed them intermittently and the log says so. Now is the time to push. Pushing registers your changes on the remote repository. So in the tragic case of you losing your computer for example, you will always have access to those changes 

`git push origin playground`

Now your branch is saved in the remote repository.

**10. Merge:** Merging is an attempt to include your branch changes to the rest of the team's. Like asking your room be part of the house. Typically, in a team setting, you would make a merge request on Github or the equivalent that your company uses. A merge request is you asking that your playground branch be included as part of the develop branch that the rest of team is.  But in the unlikely case where you have to handle this yourself, all it involves is: 

`git checkout develop`
`git merge playground`

## Conclusion

This is by no means the end to git. But this is likely to be your most typical workflow when working with git as a designer. However, understanding these 10 commands will help you work effectively with git. But just incase it all seems so tedious with the command line interface, you can also use apps such as the GitHub desktop app if your team's repository is hosted on Github. All the best with git!
