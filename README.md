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

**GENERAL NOTE** You cannot open a screen from 2 devices

## Command 6: To open jupyter notebook in a screen
- Quoted from (this answer)[https://stackoverflow.com/questions/45835971/persistent-use-of-jupyter-notebook-from-remote-server]
1. On your computer (SSH terminal; e.g. gitBash): `ssh -L xxxx:localhost:yyyy server`.
2. screen.
3. `jupyter notebook --no-browser --port=yyyy`. [on remote server]
4. In your browser: localhost:xxxx.

## Command 7: Other options while having jupyter notebook on a screen

1. To disconnect manually and reconnect: Exit the screen window: `control + a` and then `d`.
2. Disconnect from the server: `control + d` And reconnect `ssh -L xxxx:localhost:yyyy`.
- Optionally, you can reopen the screen window using `screen -r`. Go back to your notebook or reopen localhost:xxxx