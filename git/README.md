# Git


## What is Git?
From Git's own website, Git is described as "a free and open source distributed version control system designed to handle everything from small to very large projects with speed and efficiency." In layperson's terms, it's by far the most popular way that software developers collaborate with one another's code in what we refer to as **Git repositories**. Git will version your code files in a way that you can easily roll back to a previous version if required, and the way the versioning works doesn't replicate a new version of your file every single time. Instead, it will store just the changes you made to an existing file (which we refer to as **deltas**), so those deltas take up a lot less computer storage than if you were to store a full, new copy of a changed file each time.

Git should NOT be confused with other products like GitHub or GitLab. As those products' names imply, they are built on top of Git, but Git in and of itself is its own thing. While many products are designed to work with Git, I specifically call out **GitHub** and **GitLab** as they are two of the largest products that many software developers use. Here's a brief description of each:

- **GitHub**: Owned by Microsoft, GitHub is by far the most popular website for storing and sharing Git repositories. There is a free tier and paid tier (known as GitHub Pro), and most individual developers, including myself, simply use the free tier. I **VERY** highly recommend you create a GitHub profile for yourself as it is a fantastic way to showcase your work as a coding portfolio!
- **GitLab**: Whereas GitHub is generally more open to the public, many companies use GitLab as a way for their developers to store their code repositories in a more private space. In addition to repository storage, GitLab is known for their **CI/CD capabilities.** CI/CD stands for "code integration / code deployment," and it's basically this principle of creating automated code pipelines that will properly integrate your code with those of others and deploy it out to some production environment. So in essence, GitLab will allow you to store your code within it, and when the proper mechanism is triggered, GitLab will run a CI/CD pipeline to do everything it needs to do to deploy your code out into production! GitLab does have a free, web-based tier, but it's generally pretty limited. I'd still recommend it for individuals wanting to learn, but a large corporation would do well to pay for all the GitLab premium features.



## Installation on Mac and Windows
Fortunately, Git is one of the easiest tools we can download on both Mac and Windows. All you have to do is [download the installer from the Git "Downloads" page](https://git-scm.com/downloads) for your respective operating system and then follow the simple instructions after launching the installer, just as you would any other program, like Microsoft Office or Google Chrome

(*NOTE FOR WINDOWS USERS*: In a live stream I did in early January 2022, I recommended installing `Git Bash` alongside Git as that was an option in the installation steps. Git Bash is another option to use as a command line tool, but you'll see in the "Command Line Interface" tutorial, I actually recommend using `Windows Terminal` instead. It won't hurt your computer to go ahead and install `Git Bash`, but if you want to save a little computer disk space, you can skip installing `Git Bash`.)



## Basic Git Commands
In this section, I provide a few basic commands used most commonly by Git users. Now, this section honestly isn't going to make much sense to you if you've never used Git. To that end, I would very highly recommend this free course on Udacity: [Version Control with Git](https://www.udacity.com/course/version-control-with-git--ud123). You can easily knock out that course in an hour or two, and you return, these commands below will make a lot more sense to you. 😃 Keep in mind, I only note a handful of commands I use daily. There are a lot more that you should probably learn. That Udacity course will definitely cover them all, and I'm sure you can find a more robust Git command list out on the web somewhere.

- `git init`: As you can probably guess, this command officially initializes a Git repository in whatever directory in which the command is run!
- `git add`: When you make an edit to any file in your Git repository, it is not staged to be committed by default. This is so that if you make adjustments to multiple files and only want to officially commit one, you can stage just that one and leave the others be. So long as you don't discard those unstaged files, they will also remain changed on your local machine!
  - One super common flag I use is `--all` with the `git add` command. As the name implies, this will go ahead and stage all files that have been changed. Personally, I've never had a reason to stage just one change at a time, especially because I'm a frequent committer. So 99% of the time, I run the full `git add --all` command.
- `git commit`: After code has been staged with the `git add` command, this command officially commits your code to your repository. It's more or less putting the "seal of approval" on the code you've been working on.
  - A flag I always use in tandem with `git commit` is `-m`. The `-m` flag stands for "message," and it is the plain language description of the code you are making in this Git commit. So for example, it could be "Updating color on webpage." If you don't use this flag, it'll open your computer's code editor and ask you to write that commit message. I found that having to start a program for a 2 second task was super annoying, so using the `-m` flag helped a lot with that. For example, if I wanted to do a Git commit with that same message typed above, the full command would look like this: `git commit -m 'Updating color on webpage'`. Simple!
- `git push`: Even though your code is committed on your local computer, that does NOT mean your code in your source repository is automatically updated! Remember that most developers will use something like GitHub or GitLab to store all their code. In order to get your committed code from your local machine up into a place like GitHub or GitLab, you use the `git push` command!
- `git branch`: One of the nicest thing about Git is that you can continue to work on your own code without the worry of altering your main (formerly master) code. We call this working in Git branches, as your code then branches off the `main` branch. As such, the command to do this is naturally `git branch`!
- `git merge`: Okay, so as you can probably guess from the previous command, this is doing exactly what you think. Whereas the `git branch` command splits off your code into a separate branch, whenever you are ready to merge your code back into the `main` branch (or another child branch), you use this `git merge` command.