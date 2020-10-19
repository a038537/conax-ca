# conax-ca

Experimental Conax compatible DVB EMMG / ECMG plus working FUNCARD file.

Edit the files for your needs. Syskey.txt,key.txt and emm.txt.

Start emmg with listening port option. 
e.g."Conax-ecmg.exe 8888"

Start your dvb muxer with csa scrambling. Configure your scrambler to connect ecmg on the port you supplied. 
Configure your muxer to inject emms for the caid 0x0b00 on a free pid and listen to an other Port for emmg. 


When the stream is running start emmg for card updates.
e.g."conax-emmg.exe 9999"

The card should get an update with scrambling keys which are supplied in key.txt

All config files should reside in the same directory as the executables. 

Burn the funcard files to your funcard. Start the_last_dakkar, connect to your Phoenix compatible card reader. 
Open perso.txt in an editor, copy and paste the hex values one after the other, and send them to your card. 

The last string should be "set to working mode". 


No further support! You know what you are doing, or you don't know. 

Have fun.
