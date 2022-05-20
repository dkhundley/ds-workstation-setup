# Package Managers / Installers
When it comes to installing software on either a Mac or Windows machine, it can transparently be a pain in the neck! It can often mean a multi-step setup that requires you to do XYZ and pray that you didn't screw something up along the way. In order to mitigate these potential disasters, people have created these two really great package managers that simplify these installation processes quite significantly! On their respective platforms, we have **chocolatey** for Windows and **homebrew** for Mac. The instructions below will walk you through how to install these. Please note that in order for you to complete these installations, you will need to have [already installed your Command Line Interface (CLI) tool.](../command-line-interface/README.md)

## Choclately (Windows Users)
The [official instructions](https://chocolatey.org/install) are actually really straightforward, but to save you a click, I've pasted them down below. Just note they'll probably more inclined than me to keep these instructions updated. 😃

1. Right-click on the "Terminal" application in your Windows start menu and click "Run As Administrator."
2. Copy and run the following line of code into your Terminal.
   - `Set-ExecutionPolicy Bypass -Scope Process -Force; [System.Net.ServicePointManager]::SecurityProtocol = [System.Net.ServicePointManager]::SecurityProtocol -bor 3072; iex ((New-Object System.Net.WebClient).DownloadString('https://community.chocolatey.org/install.ps1'))`
3. Press the Enter key.
4. Type "Y" for "Yes" when asked to do so.
5. Type `choco` and press Enter to verify your installation was a success!

## Homebrew (Mac Users)
*To be added!*