# Command Line Interface (CLI)

## What is the Command Line Interface (CLI)?
The command line interface, or CLI, is the one of the primary ways in which a software developer interacts with a computer. Most programs you are familiar with run as Graphical User Interfaces, or GUIs. (Pronounced "gooey".) As great as GUIs are, they are very subjective from program to program. For example, can you remember how to access the settings for Facebook or Twitter on your phone? Chances are they're in different places! The CLI keeps things a lot more basic, which is helpful for developers as allows for complex functionality to be run in a more simplified, text-based interface.

Mac and Windows each have their own respective CLIs, and for data science work, we're going to focus more on the Mac flavor of this. It's actually not Mac but Linux as the macOS is built on top of Linux. In case you're not aware, Linux is an operating system (OS) similar to how Windows and macOS are OSs. Linux comes in many flavors, inlcuding Debian and Ubuntu, and Linux can range from being very simple to being very complex due to its customizability. For deploying software programs to production environments, many of these software programs are run on Linux.

## Installation on Mac
As noted before, the Mac CLI already uses Linux commands, so you can actually begin immediately using the default `Terminal` application that comes bundled with every Mac. While there is nothing wrong with using the default `Terminal` application, I personally prefer to use `iTerm2`. If you would like to install `iTerm2`, navigate to this website and follow the download instructions: [Link to iTerm2 website](https://iterm2.com/).

There is more customizability we can do to `iTerm2`, but for now we're going to keep things basic. I might come back and update this Markdown at a later time with those customizability features!

## Installation on Windows
While macOS is built on top of Linux and therefore uses Linux commands right out of the box, this is not the case with Windows. By default, Windows instead makes use of its own CLI called the **Command Prompt**. Because the Command Prompt uses radically different commands from standard Linux commands, we will NOT be making use of the Command Prompt at all.

In an effort to remedy this, Microsoft has started bundling a program called **Windows Terminal** (with another program called **PowerShell** as a profile) with newer versions of Windows. Windows Terminal and PowerShell have been designed to emulate those same Linux commands we see across macOS and other Linux machines. If these are not already installed on your computer, you can install these directly from the Microsoft Store. Here are the appropriate links for those:

- [Link to install **Windows Terminal**](https://www.microsoft.com/store/productId/9N0DX20HK701)
- [Link to install **PowerShell**](https://www.microsoft.com/store/productId/9MZ1SNWT0N5D)

To actually make use of Windows Terminal with the PowerShell profile, open Windows Terminal and navigate to the settings. (The screenshot below illustrates where this is, if you can't find it!) Under the "Default profile" dropdown menu, select "PowerShell" (NOT to be confused with Windows PowerShell, which is something different). Then click the "Save" button the bottom right hand corner of the UI.

![](../admin/assets/windows-terminal-settings.png)

Technically, this is all you need to do to get Windows Terminal working, but there are some cool things we can do with Windows Terminal / PowerShell that aren't available right out of the box. If you'd like to enable these advanced features, check out the next subsection!

### Customizing Windows Terminal



## Learning Linux Commands
Linux comes with a lot of common commands that are used on a regular basis. Udacity has an excellent free course that teaches these commands well, and I would highly advise you check that out. Here is a link to that course: [Udacity - Linux Command Line Basics](https://www.udacity.com/course/linux-command-line-basics--ud595).

As a quick reference, here are some of the commands I use on a regular basis:
- **cd**: Standing for "change directory", this command helps you to traverse your computer's directory (or folder) system.
- **pwd**: Standing for "print working directory", this command will tell you which directory your CLI currently is in.
- **ls**: This command displays all files and subdirectories listed in the current directory you are working in.
- **mkdir**: Standing for "make directory", this command will create a new directory under the directory you are currently in.
- **touch**: Similar to the `mkdir` command, `touch` will create a new file under the directory you are working in.
- **rm**: Standing for "remove", this command will remove a file. Be careful when using this command!!
- **cp** and **mv**: Standing for "copy" and "move", these commands work similarly to move files or directories around. As the names imply, one is simply moving files from one place to another, whereas the the `cp` command performs a copy without moving the original file.
- **cat**: This command displays the contents of a file.