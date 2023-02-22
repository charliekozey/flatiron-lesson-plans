# Git Basics, Terminal Commands

Also featuring helpful extensions and apps, keyboard shortcuts

Open this markdown file in VS Code and use cmd-shift-V or 
alt-shift-V to open a preview and make it easier to read

# Git basics
- git != GitHub
- git = software that helps you track changes in code
- GitHub = service that hosts your repos for easier collab
  - alternatives: Sourcehut, GitLab, BitBucket
---  
## local vs. remote
- local = your computer
- remote = away on GitHub's server
- (now I will draw a diagram)
---
## repository
 - ```.git``` file is what makes it a git repo
---
## branch vs. fork vs. clone
- branch = a tree branch
- fork = making an exact copy of the tree
  - still has a way to pull information from the old tree
- clone = planting it in your own yard (local repository)
---
## looking forward (project week)
- main vs other branches --> more on this later
- add, commit, push --> also more later
- ```git status``` is your friend
---

# Terminal 101

## "directory" == "folder"
---
## $
- you'll often see in code examples online 
- indicates "this is what you type in the terminal"
- don't include it if you copy/paste
---
## ~
- represents your root directory
- on Mac, this is Yourname (with Home icon) by default
  ```bash
  $ /Users/yourname
  ```
- on Windows Subsystem for Linux, this is the root of your Ubuntu system: 
  
  ```bash
  $ \\wsl$\Ubuntu
  ```
---
## . (a single period)
- represents "this folder you're in right now"
- for example, to open a folder in VS Code:
  ```bash
  $ code .
  ```
  ---
## .. (two periods)

- represents "the folder one level above this one"
- for example, to open an enclosing folder in VS Code:
  ```bash
  $ code .
  ```
---
## cd
- stands for "change directory"
- lets you move around your folder structure
- to move up one directory:

  ```bash
  $ cd ..
  ```

- to move to your root directory: 
  
  ```bash
  $ cd ~
  
  ```

- OR just...
  
  ```bash
  $ cd
  ```

- to move to a specific directory:
  
  ```bash
  $ cd ./nested_folder
  ```
---
## ls

- lists the contents of the current directory
  
  - super useful

```bash
$ ls
```
---
## pwd
- stands for "print working directory"
- useful for orienting yourself in the file tree
  
  ```bash
  $ pwd
  ```
---
## mkdir
- "make directory"
- creates a new folder inside the current folder
  
  ```bash
  $ mkdir new-folder-name
  ```
## touch

- like "mkdir" except it makes a new file
  
  ```bash
  $ touch README.md
  ```
## rm

- remove the specified file
- must run command from inside the folder where the file is
- PERMANENTLY DELETES THE FILE SO BE CAREFUL
  ```bash
  $ rm file-to-delete.js
  ```
- it will ask for confirmation so you must then press y or n
- to avoid the confirmation dialog, use `$ rm -f` (-f for "force")

## rm -r
- remove the specified folder
- "-r" is a *flag* that means "recursive"
- basically it allows you to delete a whole folder at once
- again, PERMANENTLY DELETES THE FOLDER SO BE CAREFUL
  ```bash
  $ rm -r folder-to-delete
  ```
- it will ask for confirmation so you must then press y or n
- to avoid the confirmation dialog, use ``` $ rm -rf ``` (-f for "force")
---
## Organized folder structure

1. open your terminal
2. use the terminal commands above to practice navigating your file tree
3. if you haven't already, use terminal commands to build something like:
   - ~       
     - Code
       - prework
       - phase_1
       - phase_2
       - phase_3
       - phase_4
       - phase_5

4 you can then ```$ git clone``` all of your labs and projects into the corresponding folder
5 it really helps to have an organized system! future you will appreciate it when you're looking for things later
---
## Keyboard shortcuts:

## switch between apps quickly

cmd-tab (Mac) or alt-tab (PC)

## switch between windows of same app

cmd-\` (Mac) or alt-\` (PC)

(the ` key is at the upper left corner of the keyboard)

---
## Apps and Extensions:

### make your terminal easier to read & navigate: 

- [oh my zsh](https://ohmyz.sh/)

### tile and snap your app windows around quickly

- for Mac: [rectangle](https://rectangleapp.com/)

- on Windows: just use ```windows key + arrow keys```

### tab out (VS Code extension)

https://marketplace.visualstudio.com/items?itemName=albert.TabOut


