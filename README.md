# Twenty-Twenty-Notify
A useful tool, to relax our eyes from constant strain by computer screen.The application send a notification which says “blink your eyes” in an interval of 20 minutes.

##How to setup Twenty-Twenty-Notify
1. `ctrl + alt + t` : This opens a terminal in ubuntu.
2. Move to directory where you have clone this repository.
3. Change the directory to the file containg trail.sh.
4. Use this command to add executable permission to trail.sh file.
   `chmod +x trail.sh`
5. Now we will edit the contents of the cronjob file, for this type in the command.
   `crontab -e`
6. Terminal will promt you choose an appropriate editior, if no default editor is set.
7. Copy the location of you trail.sh file, in my case the location is /home/sajal/twenty_twenty/trial.sh.
8. Append the below given line at the end of crontab-e file:
   `*/20 * * * * env DISPLAY=:0 /home/sajal/twenty_twenty/trial.sh`
9. Now sit back,read ebooks or surf the web, now your computer will help you take care of your beautiful eyes.
