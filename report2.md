# Lab Report 2 - Servers and SSH Keys
## Part 1 - Chat Server
### 1A - Code
![Image](https://bryab-edu.github.io/cse15l-lab-reports/report2files/codeShot1.PNG)
![Image](https://bryab-edu.github.io/cse15l-lab-reports/report2files/codeShot2.PNG)
### 1B - Page
#### ![Image](https://bryab-edu.github.io/cse15l-lab-reports/report2files/pageShot1.PNG)
This page is the result of the handleRequest method. The one argument being used is the websites URL it produces. The values being used are
1. `log` the String that acts as the concantation of the message and the user Strings. `<username>: <message>`
2. `msgUsr` the String list that helps represents the Query in which splits the username and message strings (Both: `jpolitz` and `Hello`)
3. `msg` the message String isolated `"Hello"`
- `chatLogs` - the one modified String that acts as the database for all the messages being added, log is added (`jpolitz: Hello`)
#### ![Image](https://bryab-edu.github.io/cse15l-lab-reports/report2files/pageShot2.PNG)
This page is also the result of the handleRequest method. The one argument being used is the websites URL it produces. The values being used are
1. `log` the String that acts as the concantation of the message and the user Strings. `<username>: <message>`
2. `msgUsr` the String list that helps represents the Query in which splits the username and message strings (Both: `yash` and `How are you`)
3. `msg` the message String isolated `"How are you"`
- `chatLogs` - the one modified String that acts as the database for all the messages being added, log is added (`yash: How are you`). Now that there's multiple logs, each log is split up by the formatting, using `%n` to put each new log onto the next line.
## Part 2
## Generated Key Directory
#### ![Image](https://bryab-edu.github.io/cse15l-lab-reports/report2files/terminalShot1.PNG)
## Generated Key Directory contents (private key is the non-.pub file)
#### ![Image](https://bryab-edu.github.io/cse15l-lab-reports/report2files/terminalShot4.PNG)
## Executing ssh-keygen command to save public key (.pub file)
#### ![Image](https://bryab-edu.github.io/cse15l-lab-reports/report2files/terminalShot2.PNG)
#### ![Image](https://bryab-edu.github.io/cse15l-lab-reports/report2files/terminalShot3.PNG)
## Part 3 - Week 2/3 Reflection
I learned about a some of things during the past couple labs. I learned how to make a small Server online through localhost. I learned how to connect to my student account through the terminal. Most importantly, I leanred more on how to navigate and create on github, such as creating a repository and representing it through pages. 
