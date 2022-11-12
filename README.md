# GitLyra

This is a for my course in Server Managment assignment h3
This assignemnt is a part of a-e assignment and you can find the assugnment in: https://terokarvinen.com/2022/palvelinten-hallinta-2022p2/?from=MoodleNews#h3-git
I have also used My own notes I have done. 
## a) Do this assignment in markdown and use GitHub
I created for this assignment a respository called GitLyra. I already had an account so it was easy. 

##b)Offline, create a offline respository on your VM. The name has to containg "cat".

I started with updating my VM. I dont have Git in this Vm so next Thing I did is to install Git on it.
  $sudo apt-get install git
Next I made a directory called catlyra. 
  $git init catlyra
The direcory was created: 
  /home/Lyra/catlyra/.git/
Next I'm supposed to do changes in the direktory and show the changes. 
I chose to check that the direktory was created and moved in to the directory

  $ls
  $ cs catlyra/
  
I chose to create a nano text file here. 

  $nano catlyragit

I added -Cat Lyra Git- in the nano text file, saved and closed. 

  $cat catlyragit
 
I wanted to check that I actually wrote the text so that I don't get to problems later if it don't show. Test in small pices while you do. Easier in case of issues of misstakes that always get made.
After this I used the commands under to add and register the name and e-mail. 

Next I added the changes and committed them. 
  $git add .
  $git commit

After this it asked me to identify myself so I addedmy mail and name. 

  $git config --global user.mail"muns.steinmetz@gmail.com"
  $git config --global user.name "Marie-Helene Steinmetz"
  
After this I ran:
  $git commit
  
Added a note in the commit log. 
First note in catlyra

I got a confirmateion that it actually worked. 
Next I want to check the log.
  $git log --patch

The log showed that I added text, added a note, my name and mail. 

c) Make stupic misstakes in Git and check them in logs

I chose to add text to my catlyragit and the run th ecommit without add. This way it did not add the commit note in the right place. It did not see in the log either anything. 

d) Make a new repositori in Github with the word "car" in the name and description. 

I made a  README.md and used a free licensen GPLv3 (GNU General Public License version 3)

e)Dolly. Kloonaa edellisessä kohdassa tehty varasto itsellesi, tee muutoksia, puske ne palvelimelle, ja näytä, että ne ilmestyvät weppiliittymään.

I cretaed a new direktory, carlyragit, added text, and then created a SSH key
  $ssh-keygen #3 times return.
  
  $cd /home/lyrs/.ssh #here I can see to different keys. One is the secret that I will not open and the other is the publi so I wil use "cat" to show it to me and copy it to my github page:
  $cat id_rsa.pub



I did not find in GitHub where to add the SSH key. So Google it is. 

"How to Add an SSH Key to your Github Account
Log into your GitHub account.
Click your avatar and choose Settings.
Select SSH and GPG keys.
Click New SSH key.
Enter a title in the field.
Paste your public key into the Key field.
Click Add SSH key."

https://www.inmotionhosting.com/support/server/ssh/how-to-add-ssh-keys-to-your-github-account/

I added the key in Github and after that I cloned the repository to my VM.

git@github.com:Marie-HeleneSteinmetz/CarLyra.git

I first went to the cloned department CarLyra and used
 $ cd pull
It was up to date.Then I wrote content in the README.md.

 $cd add .
 $cd commit #added a comment in logs
 $ cd pull
 $ cd push
 $ git log --patch #to check that it all came in.

I updated the GitHub page, cjecked log, added text and note and then I did thepull in terminal to see if it workd. 

