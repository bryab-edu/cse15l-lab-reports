# Lab Report 4
## 1. Using Bash History (up/down arrows)
![Image](https://bryab-edu.github.io/cse15l-lab-reports/report4files/bashscreenshot1.PNG)
In this first image I typed the commands `javac ListExmaples.java` and `java ListExamples` accordingly
![Image](https://bryab-edu.github.io/cse15l-lab-reports/report4files/bashscreenshot2.PNG)
Keys pressed: `<Ctrl+r>`, by searching using keyword `java` the command `java ListExamples` my most recent command entered shows up.
![Image](https://bryab-edu.github.io/cse15l-lab-reports/report4files/bashscreenshot3.PNG)
Keys pressed: `<up>` I now scroll through the previous command using the `<up>` directional key to go back to another command I entered with keyword `java` and so `javac ListExmaples.java` shows up
![Image](https://bryab-edu.github.io/cse15l-lab-reports/report4files/bashscreenshot4.PNG)
Keys pressed: `<down>` now, to go back to newer entries of commands using the keyword `java` I can go back to `java ListExamples` using the `<down>` directional key

## 2. Using Tab
Before
![Image](https://bryab-edu.github.io/cse15l-lab-reports/report4files/bashscreenshot5.PNG)
After
![Image](https://bryab-edu.github.io/cse15l-lab-reports/report4files/bashscreenshot6.PNG)
Keys pressed: `<tab>` using `<tab>` after a command in this context, would search for a file using keyword `List` like `ListExamples`. By typing a portion of the file I can autocomplete it by typing in `<tab>`.
![Image](https://bryab-edu.github.io/cse15l-lab-reports/report4files/bashscreenshot5.5.PNG)
Keys pressed: `<tab><tab>` if I were to press `<tab>` once again, I would be provided with multiple versions of a file named `ListExamples` but with different file types. There, bash narrows down the options even further. 
![Image](https://bryab-edu.github.io/cse15l-lab-reports/report4files/bashscreenshot7.01.PNG)
Keys pressed: `<tab>` in this context of autocompleting a command and I want `java`, by pressing `<tab>` once, nothing happens. Why not?
![Image](https://bryab-edu.github.io/cse15l-lab-reports/report4files/bashscreenshot7.02.PNG)
Keys pressed: `<tab><tab>` well, thats because the starting key `ja` already provides many current commands the user may not have been aware of and acts as if I had `ListExamples` instead of `List`. Thus, by pressing `<tab>` once more, I'd be provided with many options for not only commands but other misc files.

## 3. Keyboard Shortcuts while editing commands
### `<Ctrl+U>` - Erases everything previous to the cursor
Before - Ah darnit!!! I mispelled javac as jacac!!! I'll never recover... :(
![Image](https://bryab-edu.github.io/cse15l-lab-reports/report4files/bashscreenshot8.PNG)
After (Press `<Ctrl+u>`) - Gone
![Image](https://bryab-edu.github.io/cse15l-lab-reports/report4files/bashscreenshot9.PNG)
### `<Ctrl+k>` - Erases everything following the cursor
Before
![Image](https://bryab-edu.github.io/cse15l-lab-reports/report4files/bashscreenshot10.PNG)
After (Press `<Ctrl+k>`)
![Image](https://bryab-edu.github.io/cse15l-lab-reports/report4files/bashscreenshot10.PNG)
### `<Ctrl+a>` - Moves cursor to the beginning of the line
Before



