# Pico-Ducky-Fix-files
Files to a possible fix for Pico Ducky not working

Hey. I've seen a few people saying their Rasberry Pi Pico is not working for the Pico Ducky mod.  I found a fix and tried commenting on it on the post. It won't let me add files so I am reposting it here. I hope that's alright. I'm new to Reddit so if this is not a good thing to do please accept my sincere apologies. Here is what I said in the comment. Files linked (hopefully :)

After one year of no answer on this Reddit post, I think I've found a solution for this. It's not the best but it seems to work as it is supposed to. The only downside is that you won't get the newest features (multi-payload and whatever else) and possible bug fixes. Before I start I just want to mention I am new to Reddit and may not know how to properly give info or solve stuff like this. Except for my sincere apologies if I did it wrong:) Here is the fix I found that worked for me:

So back in the winter of 2023, I had a Hacking class where we used this. The teacher gave out the files we needed (normally you go to GitHub and download the lib file and only take 4-6 files and move them to lib and base of the Pico. The teacher just gave the needed files to make it easier.). Now these files are from the older version and the files that needed to be moved may not have the newest updates on them. Now the issue I've had and it seems like others are having is with the newest files it won't work. I've seen comments saying to turn safe mode on before setting up Pico and I did that it didn't work. So I tried using these old files instead of the newest ones. Surprisingly, it worked. The files are there somewhere wherever Reddit puts them and they go in libraries as follows (EDIT: There is a link I can't upload some files. (prob on GitHub)😭): 

adafruit-circuitpython-raspberry_pi_pico-en_US-7.3.3 = This is what you should put in the VERY BEGINNING WHEN YOUR PICO IS CLEAN AND HAS NO PICO-DUCKY FILES ON IT (on a hard reset). This sets up the pico so it's a pico-ducky. Now after this, we add more files into the lib folder and the root of the pico

payload.dd = This is where you put your code. It goes into the base/root of the Raspberry Pi Pico

lib.zip = extract this and inside you find 4 files. These 4 files go to the lib folder in the pico-ducky's files.

old code.py that is already there from the pico-ducky install

boot.py = This should go into the root of the pico as well. 

Once done you can go into payload.dd. It should already be set up for a hello world type into a notepad. It should only activate the code and do the job it's supposed to (typing hello world in this case) when it's all set up and the device is disconnected and reconnected. You don't have to take this payload.dd you can just make your own or find some on the Hak5 website. Just remember, as my teacher said, MAKE SURE ITS NAMED "payload.dd". THE NAME IS IMPORTANT! 

This may fix the issue of the Pico Ducky not working after doing the newest steps from the official devs. I'm just clarifying that this is not my code it's the code of dbisu on https://github.com/dbisu/pico-ducky?tab=readme-ov-file. I'm just putting older files that work for me and maybe others here so I can use this to link to a Reddit post. If I'm doing anything wrong, my apologies, I'm new to Github and Reddit. 
