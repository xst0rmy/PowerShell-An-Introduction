# PowerShell-An-Introduction
Prior to today, I didn't know PowerShell had such great potentials. I want to share some cool stuffs about PowerShell... Hopefully, you learn to love PowerShell as am learning to. I will also create other PowerShell repositories about other features I learn. 

> **First things first, Always run PowerShell as Administrator. It gives you an unrestricted access to all PowerShell funtionalities, so why not?**

![](https://github.com/xst0rmy/PowerShell-An-Introduction/blob/main/Images/Screenshot%202023-01-28%20at%2007.14.41.png)

> **Always start your PowerShell session with a "Start-Transcipt" command if for any reason you wish to go through all you've done in that session. I'll talk more on this later on.**

![](https://github.com/xst0rmy/PowerShell-An-Introduction/blob/main/Images/pshell%201.png)

> **Did you noticed how the first command was written as "Start-Transcript". I'll use that example to describe the verb-noun assignment commands. Most PowerShell commands are written in a way that helps the reader understand what that command would likely perform. Commands in Powershell are easy to write out and execute when they are in the verb-noun state.**

> **It also important to note that PowerShell is case-insensitive. The "Tab" key on the keyboard can be used to automatically select a command after you've written some letters (keep clicking the tab key till you get the command you want). I will suggest you use the tab key in the noun section of the command because the verb section of PowerShell commands have numerous similar starting commands). Using the "Tab" key to auto-generate a command produces the command with the first alphabet of the verb-noun words in Capital Letters.**

> **PowerShell has so many commands to use and fortunately, we don't have to memorize it all. we can easily use the "get-command" as used in the image below**

![](https://github.com/xst0rmy/PowerShell-An-Introduction/blob/main/Images/pshell%202.png)

> **It produced sooo many commands as seen below. The scrolling bar at the right shows how much more commands there are if you keep scrolling down.**  

![](https://github.com/xst0rmy/PowerShell-An-Introduction/blob/main/Images/pshell%203.png)

*Remember what I wrote about using the Tab button on keyboard to auto-complete a command. With the image above, you wouldn't want to type only the verb command and use the tab key as there so many similar verb command but you can do that if you're sure the verb command doesn't have so many similar commands.

> **Using the "get-command" is not entirely advisable to use if your aim is not to go through all the available commands you can use in PowerShell. A better option is to call up a more specific command with the "get-command" command**

![](https://github.com/xst0rmy/PowerShell-An-Introduction/blob/main/Images/pshell%204.png)

*The above command produced only commands with "SystemLanguage"

> **If you ever get curious on what a PowerShell command is meant to do, use the "get-help' command as shown below**

![](https://github.com/xst0rmy/PowerShell-An-Introduction/blob/main/Images/pshell%205.png)

*You will most likely be presented with that question after inputing the "get-help" command. That gives you the opprtunity to update your PowerShell help files with the latest additions. so go ahead and input "y"

> **The "get-help" option gives an elaborate description of a command and the various ways it can be used in a syntax. I'll explain further what the "Aliase" means shortly. The reference option underlined in the image is a path to getting more information from the web in a GUI (Graphical User Interface) format. Running that command on PowerShell opens up your browser and shows you more information on that command**  

![](https://github.com/xst0rmy/PowerShell-An-Introduction/blob/main/Images/pshell%206.png)

*What are Aliases? Aliases are cfommands that can be run on PowerShell but they don't follow the verb-noun rule. In a way, they arw abbreviations of a command. If you are familiar with the basic either Windows Command Prompt or Linux Terminal command, some of the basic commands used on those terminals can be found as aliases on PowerShell.

> **In the image below, "cls" is an alaise to clear-host which clears your screen**

![](https://github.com/xst0rmy/PowerShell-An-Introduction/blob/main/Images/pshell%207.png)

![](https://github.com/xst0rmy/PowerShell-An-Introduction/blob/main/Images/pshell%208.png)

> **Wondering what an alaise means? Use the "get-alaise" command**

![](https://github.com/xst0rmy/PowerShell-An-Introduction/blob/main/Images/pshell%209.png)

![](https://github.com/xst0rmy/PowerShell-An-Introduction/blob/main/Images/pshell%2010.png)

> **Wondering what other aliase is at your disposal?**

![](https://github.com/xst0rmy/PowerShell-An-Introduction/blob/main/Images/pshell%2011.png)

> **Use the "grt-process" command to see a comprehensive list of all runnung processes of your PC**

![](https://github.com/xst0rmy/PowerShell-An-Introduction/blob/main/Images/pshell%2012.png)

> **To view a specific process, use the command in the image below

![](https://github.com/xst0rmy/PowerShell-An-Introduction/blob/main/Images/pshell%2013.png)


> **The commands in the syntax below gets the information about "system" and pipes "|" it to the "get-member" command which means it takes the result from the "get-process" over to the "get-member" command to display the results shown in the image below. The result shows various methods (different things you can do with the command) and properties (description of the command), various associated aliases and other vital information regarding how to efficiently use the command.**

![](https://github.com/xst0rmy/PowerShell-An-Introduction/blob/main/Images/pshell%2014.png)

> **In the image below,I made a vital omission in the first two command while trying to display the properties of a process. At first, I didn't realise ommiting the asterisks sign * was the problem until i figured it out as shown in the image below**

![](https://github.com/xst0rmy/PowerShell-An-Introduction/blob/main/Images/pshell%2015.png)

> **What do you know about Variables in programming? Well, I know variables as a basic explanation is used to assigned values to an object.**

> **In PowerShell, the dollar sign $ is used to represent a variable and a value is assigned to that variable object with an equal to sign "=" as shown in the image below**

![](https://github.com/xst0rmy/PowerShell-An-Introduction/blob/main/Images/pshell%2016.png)

> **In the image below, I assigned "$storm" to represent the  "get-process system" command which means that in the future, whenever I write out $storm, PowerShell will understand that I am asking for the process of system to be displayed.**

![](https://github.com/xst0rmy/PowerShell-An-Introduction/blob/main/Images/pshell%2017.png)

> **I went ahead to input other commands using the assigned variable in my previous example and shows the result in the image below**

![](https://github.com/xst0rmy/PowerShell-An-Introduction/blob/main/Images/pshell%2018.png)

> **Curious with what commands you've used all through a session? Use the "get-history" command to see a complete list of all commands you typed on your keyboard so far. Here is an example in the image below

![](https://github.com/xst0rmy/PowerShell-An-Introduction/blob/main/Images/pshell%2019.png)

> **At the beginning of this repo, you read about the "start-transcript" command. This command is similar to the "get-history" command, but it's very much detailed to include the results each command you used provided and it is stored in your document folder on your PC.

![](https://github.com/xst0rmy/PowerShell-An-Introduction/blob/main/Images/pshell%2021.png)

![](https://github.com/xst0rmy/PowerShell-An-Introduction/blob/main/Images/pshell%2022.png)


















