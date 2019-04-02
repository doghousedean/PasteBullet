# README #

### What is this repository for? ###

This will send your piped data to termbin.com and then push you the link via pushbullet, having pushbullet chrome addon is helpful

### How do I get set up? ###

1) clone the repo

2) edit notify_pushbullet to include your API key from pushbullet

3) create symlinks to both files in /usr/local/bin so you can call them anywhere

4) use it

#### Details ####

1)

	$ git clone git@github.com:doghousedean/PasteBullet.git
	
2)

	Get your API key from https://www.pushbullet.com/#settings/account
	Click create token and copy it
	
	$ vim notify_pushbullet
	
	update the apikey variable to have your key, save and quit
	
3)

	$ cd /usr/local/bin
	$ ln -s ~/pastebullet/notify_pushbullet .
	$ ln -s ~/pastebullet/term_bin .
	

### Examples for use, just a few ###
	
	$ cat readme | term_bin
	$ grep "interesting info" large_doc | term_bin
	$ cat data.csv | term_bin
	

### Contribution guidelines ###

* knock yourself out! 
