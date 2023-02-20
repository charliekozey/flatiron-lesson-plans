# Terminal Commands, Helpful Extensions and Apps, Keyboard Shortcuts

***

### TIP!! Open this markdown file in VS code and use cmd-shift-V or alt-shift-V to open a preview and make it easier to read

*** 

# Terminal 101

## "directory" == "folder"

## $

- you'll often see in code examples online 

- indicates "this is what you type in the terminal"

- don't include it if you copy/paste

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

## . (a single period)

- represents "this folder you're in right now"

- for example, to open a folder in VS Code:
  
  ```bash
  $ code .
  ```

## .. (two periods)

- represents "the folder one level above this one"

- for example, to open an enclosing folder in VS Code:
  
  ```bash
  $ code .
  ```

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

## ls

- lists the contents of the current directory
  
  - super useful

```bash
$ ls
```

![Screen Shot 2022-11-21 at 11.13.00 AM.png](/Users/charliekozey-flatiron/Desktop/Screen%20Shot%202022-11-21%20at%2011.13.00%20AM.png)
 

## pwd

- stands for "print working directory"

- useful for orienting yourself in the file tree
  
  ```bash
  $ pwd
  ```

![Screen Shot 2022-11-21 at 11.14.51 AM.png](/Users/charliekozey-flatiron/Desktop/Screen%20Shot%202022-11-21%20at%2011.14.51%20AM.png)

## mkdir

- "make directory"

- creates a new folder inside the current folder
  
  ```bash
  $ mkdir new-folder-name
  ```

![Screen Shot 2022-11-21 at 11.17.54 AM.png](/Users/charliekozey-flatiron/Desktop/Screen%20Shot%202022-11-21%20at%2011.17.54%20AM.png)

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
  $ rm folder-to-delete
  ```

- it will ask for confirmation so you must then press y or n

- to avoid the confirmation dialog, use ``` $ rm -rf ``` (-f for "force")


## Organized folder structure

1. open your terminal

2. use the terminal commands above to practice navigating your file tree

3. if you haven't already, use the terminal commands to create the following file structure:
   
   - ~    
     
     - Documents (or just put your Code folder right in ~)
       
       - Code
         
         - prework
         
         - phase_1
         
         - phase_2
         
         - phase_3
         
         - phase_4
         
         - phase_5

4- you can then ```$ git clone``` all of your labs and projects into the corresponding folder

5- it really helps to have an organized system! future you will appreciate it when you're looking for things later

## Apps and Extensions:

### make your terminal easier to read & navigate: 

- [oh my zsh](https://ohmyz.sh/)

### tile and snap your app windows around quickly

- for Mac: [rectangle](https://rectangleapp.com/)

- on Windows: just use ```windows key + arrow keys```

### tab out (VS Code extension)

https://marketplace.visualstudio.com/items?itemName=albert.TabOut


## Keyboard shortcuts:

## switch between apps quickly

cmd-tab (Mac) or alt-tab (PC)

## switch between windows of same app

cmd-\` (Mac) or alt-\` (PC)

(the ` key is at the upper left corner of the keyboard)

