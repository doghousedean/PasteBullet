# README #

### What is this repository for? ###

This will send your piped data to termbin.com and then push you the link via pushbullet, having pushbullet chrome addon is helpful

### How do I get set up? ###

1) clone the repo

2) edit notify_pushbullet to include your API key from pushbullet

3) create symlinks to both files in /usr/local/bin so you can call them anywhere

4) use it

1)

	$ git clone git clone git@bitbucket.org:doghousedean/pastebullet.git
	
2)

	Get your API key from https://www.pushbullet.com/#settings/account
	Click create token and copy it
	
	$ vim notify_pushbullet
	
	update the apikey variable to have your key, save and quit
	
3)

	$ cd /usr/local/bin
	$ ln -s ~/pastebullet/notify_pushbullet .
	$ ln -s ~/pastebullet/term_bin .
	
	
4)
	Examples for use, just a few
	
	a) $ cat readme | term_bin
	b) $ grep "interesting info" large_doc | term_bin
	c) $ cat data.csv | term_bin
	

### Contribution guidelines ###

* knock yourself out!