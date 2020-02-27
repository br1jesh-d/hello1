	findstr /misp "multipart/form-data" pathname\*.* > upload-ServerIP.txt 
	findstr /misp "username password" pathname\*.* > logins-ServerIP.txt 
	dir /s /b pathname\*.txt pathname\*.sql > extra-ServerIP.txt 
	dir /b /ad pathname\*.* > list-ServerIP.txt 
	dir /s /b pathname\*.asp* | findstr ";" > sus-ServerIP.txt 
	dir pathname /s/b > all_files.txt 
NOTE: 
1)	Replace pathname with the location where the web applications are hosted. 
2)	Replace ServerIP with the webservers' Public IP/IPs. 
3)	Zip the output files generated from the above commands and send it to us.
4)      And then delete all the output files generated from above commands and No data/information 
should be left at the server related to the above activity.
