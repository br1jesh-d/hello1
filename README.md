Windows Web Server:
Run the following command on cmd and provide us its output files such as upload-ServerIP.txt, logins-ServerIP.txt,
extra-ServerIP.txt, list-ServerIP.txt, sus-ServerIP.txt and all_files.txt.

1.	findstr /misp "multipart/form-data" pathname\*.* > upload-ServerIP.txt 
2.	findstr /misp "username password" pathname\*.* > logins-ServerIP.txt 
3.	dir /s /b pathname\*.txt pathname\*.sql > extra-ServerIP.txt 
4.	dir /b /ad pathname\*.* > list-ServerIP.txt 
5.	dir /s /b pathname\*.asp* | findstr ";" > sus-ServerIP.txt 
6.	dir pathname /s/b > all_files.txt 


NOTE: 
1)	Replace pathname with the location where the web applications are hosted. 
2)	Replace ServerIP with the webservers' Public IP/IPs. 
3)	Zip the output files generated from the above commands and send it to us.
4)      And then delete all the output files generated from above commands and No data/information 
should be left at the server related to the above activity.
