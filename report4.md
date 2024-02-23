# Lab Report 4
## 1. Using Bash History (up/down arrows) <br />
![Image](https://bryab-edu.github.io/cse15l-lab-reports/report4files/bashscreenshot1.PNG) <br /><br />
In this first image I typed the commands `javac ListExmaples.java` and `java ListExamples` accordingly <br /><br />
![Image](https://bryab-edu.github.io/cse15l-lab-reports/report4files/bashscreenshot2.PNG) <br /> <br /> 
Keys pressed: `<Ctrl+r>`, by searching using keyword `java` the command `java ListExamples` my most recent command entered shows up. <br />
![Image](https://bryab-edu.github.io/cse15l-lab-reports/report4files/bashscreenshot3.PNG) <br />  <br />
Keys pressed: `<up>` I now scroll through the previous command using the `<up>` directional key to go back to another command I entered with keyword `java` and so `javac ListExmaples.java` shows up <br />
![Image](https://bryab-edu.github.io/cse15l-lab-reports/report4files/bashscreenshot4.PNG) <br />  <br /> 
Keys pressed: `<down>` now, to go back to newer entries of commands using the keyword `java` I can go back to `java ListExamples` using the `<down>` directional key <br />  <br />
## 2. Using Tab
Before <br />
![Image](https://bryab-edu.github.io/cse15l-lab-reports/report4files/bashscreenshot5.PNG) <br /><br />
After <br /><br />
![Image](https://bryab-edu.github.io/cse15l-lab-reports/report4files/bashscreenshot6.PNG) <br /><br />
Keys pressed: `<tab>` using `<tab>` after a command in this context, would search for a file using keyword `List` like `ListExamples`. By typing a portion of the file I can autocomplete it by typing in `<tab>`. <br /><br /> 
![Image](https://bryab-edu.github.io/cse15l-lab-reports/report4files/bashscreenshot5.5.PNG) <br /><br />
Keys pressed: `<tab><tab>` if I were to press `<tab>` once again, I would be provided with multiple versions of a file named `ListExamples` but with different file types. There, bash narrows down the options even further. <br /><br />
![Image](https://bryab-edu.github.io/cse15l-lab-reports/report4files/bashscreenshot7.01.PNG)<br /><br />
Keys pressed: `<tab>` in this context of autocompleting a command and I want `java`, by pressing `<tab>` once, nothing happens. Why not?<br /><br />
![Image](https://bryab-edu.github.io/cse15l-lab-reports/report4files/bashscreenshot7.02.PNG)<br /><br />
Keys pressed: `<tab><tab>` well, thats because the starting key `ja` already provides many current commands the user may not have been aware of and acts as if I had `ListExamples` instead of `List`. Thus, by pressing `<tab>` once more, I'd be provided with many options for not only commands but other misc files.<br /><br />

## 3. Keyboard Shortcuts while editing commands
### `<Ctrl+U>` - Erases everything previous to the cursor
Before - Ah darnit!!! I mispelled javac as jacac!!! I'll never recover... :(<br /><br />
![Image](https://bryab-edu.github.io/cse15l-lab-reports/report4files/bashscreenshot8.PNG)<br /><br />
After (Press `<Ctrl+u>`) - Gone<br /><br />
![Image](https://bryab-edu.github.io/cse15l-lab-reports/report4files/bashscreenshot9.PNG)<br /><br />
### `<Ctrl+k>` - Erases everything following the cursor
Before<br /><br />
![Image](https://bryab-edu.github.io/cse15l-lab-reports/report4files/bashscreenshot10.PNG)<br /><br />
After (Press `<Ctrl+k>`)<br /><br />
![Image](https://bryab-edu.github.io/cse15l-lab-reports/report4files/bashscreenshot11.PNG)<br /><br />
### `<Ctrl+a>` - Moves cursor to the beginning of the line
Before<br /><br />
![Image](https://bryab-edu.github.io/cse15l-lab-reports/report4files/bashscreenshot12.PNG)<br /><br />
After (Press `<Ctrl+a>`)<br /><br />
![Image](https://bryab-edu.github.io/cse15l-lab-reports/report4files/bashscreenshot13.PNG)<br /><br />
### `<Ctrl+e>` - Moves cursor to the end of the line
Before<br /><br />
![Image](https://bryab-edu.github.io/cse15l-lab-reports/report4files/bashscreenshot14.PNG)<br /><br />
After (Press `<Ctrl+e>`)<br /><br />
![Image](https://bryab-edu.github.io/cse15l-lab-reports/report4files/bashscreenshot15.PNG)<br /><br />
### `<Ctrl+w>` - Deletes the last word
Before<br /><br />
![Image](https://bryab-edu.github.io/cse15l-lab-reports/report4files/bashscreenshot15.PNG)<br /><br />
After (Press `<Ctrl+w>`)<br /><br />
![Image](https://bryab-edu.github.io/cse15l-lab-reports/report4files/bashscreenshot16.PNG)<br /><br />
### `<Alt+f>/<Alt+b>` - Goes back and forth by word
Before<br /><br />
![Image](https://bryab-edu.github.io/cse15l-lab-reports/report4files/bashscreenshot17.PNG)<br /><br />
After (Press `<Alt+f>`) forward 1 word<br /><br />
![Image](https://bryab-edu.github.io/cse15l-lab-reports/report4files/bashscreenshot18.PNG)<br /><br />
After (Press `<Alt+f><Alt+f><Alt+f><Alt+f><Alt+f><Alt+f><Alt+f><Alt+f><Alt+f>`) forward 9 words<br /><br />
![Image](https://bryab-edu.github.io/cse15l-lab-reports/report4files/bashscreenshot19.PNG)<br /><br />
After (Press `<Alt+b>`) backwards 1 word<br /><br />
![Image](https://bryab-edu.github.io/cse15l-lab-reports/report4files/bashscreenshot20.PNG)<br /><br />

## 4. Quick Copy/Paste
### Double Click and Triple Click Selections
Before<br /><br />
![Image](https://bryab-edu.github.io/cse15l-lab-reports/report4files/bashscreenshot17.PNG)<br /><br />
After (Hover over word, Press `<LClick>``<LClick>`)<br /><br />
![Image](https://bryab-edu.github.io/cse15l-lab-reports/report4files/bashscreenshot21.PNG)<br /><br />
After (Press `<LClick>``<LClick>``<LClick>`)<br /><br />
![Image](https://bryab-edu.github.io/cse15l-lab-reports/report4files/bashscreenshot22.PNG)<br /><br />
### `<Alt+Shift+Left>`/ `<Alt+Shift+Right>` select multiple words
Before<br /><br />
![Image](https://bryab-edu.github.io/cse15l-lab-reports/report4files/bashscreenshot17.PNG)<br /><br />
### `<Ctrl+c>` Copy
Before <br /><br />
![Image](https://bryab-edu.github.io/cse15l-lab-reports/report4files/bashscreenshot17.PNG)<br /><br />
After (Hover over word, Press `<LClick>``<LClick>`, `<Ctrl+c>`)<br /><br />
![Image](https://bryab-edu.github.io/cse15l-lab-reports/report4files/bashscreenshot23.PNG)<br /><br />
### `<Ctrl+v>` OR `<RClick> Paste
Before<br /><br />
![Image](https://bryab-edu.github.io/cse15l-lab-reports/report4files/bashscreenshot24.PNG)<br /><br />
After (Press `<Ctrl+v>` OR `<RClick>)<br /><br />
![Image](https://bryab-edu.github.io/cse15l-lab-reports/report4files/bashscreenshot25.PNG)<br /><br />





