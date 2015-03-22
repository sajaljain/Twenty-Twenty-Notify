# Twenty-Twenty-Notify
A useful tool, to relax our eyes from constant strain by computer screen.The application send a notification which says “blink your eyes” in an interval of 20 minutes.

How to setup use Twenty-Twenty-Notify
a) ctrl + alt + t : This open a terminal in ubuntu
b) move to director where you have clone this repository
c) change the directory to the file containg trail.sh
d) use this command to add executable permission to trail.sh file 
   chmod +x trail.sh 
e) now we will edit the contents of the cronjob file, for this type in the command
   crontab -e
f) terminal will promt you choose an appropriate editior if no default editor is set
g) copy the location of you trail.sh file in my case the location is /home/sajal/twenty_twenty/trial.sh
h) append the below given line at the end of crontab-e file:
   */20 * * * * env DISPLAY=:0 /home/sajal/twenty_twenty/trial.sh
i) Now sit back,read ebooks or surf the web, now your computer will help you take care of your beautiful eyes
