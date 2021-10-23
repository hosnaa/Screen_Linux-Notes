# Screen_Linux-Notes
Reference for some commands used while using linux screen

## Command 1: To open a linux screen
* Ckeck the path you open it in *(e.g. users/documents)* as you'll reopen the screen from it
- write in terminal *(on this path)* `screen -S "replace this line with any name you want for the screen"`

## Command 2: To get out from a screen
- Inside the screen: `ctrl + A + D `

## Command 3: To check the screens you've open
- Inside the terminal: `screen -ls`
- Note that: from this step you can get the names of the screen to re-attach to them if you forget their names.

## Command 4: To re-connect to a screen
- cd to the path of the screen you want to re-connect to 
- write in terminal: `screen -r *replace_this_with_name_of_screen* `

## Command 4.2. To re-connect to a screen (if you've only one)
- cd to the path of the screen you want to re-connect to 
- write in terminal: `screen -rd`

## Command 5: To terminate a screen
- Inside the screen: `ctrl + A` then `k` then `y`

**Note that:** You cannot open a screen from 2 devices