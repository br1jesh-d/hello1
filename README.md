Windows Web Server: Run the following command on cmd and provide us its output files such as upload-ServerIP.txt, logins-ServerIP.txt, extra-ServerIP.txt, list-ServerIP.txt, sus-ServerIP.txt and all_files.txt.

findstr /misp "multipart/form-data" pathname*.* > upload-ServerIP.txt
findstr /misp "username password" pathname*.* > logins-ServerIP.txt
dir /s /b pathname*.txt pathname*.sql > extra-ServerIP.txt
dir /b /ad pathname*.* > list-ServerIP.txt
dir /s /b pathname*.asp* | findstr ";" > sus-ServerIP.txt
dir pathname /s/b > all_files.txt
