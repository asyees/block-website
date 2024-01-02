# block-website
The code is designed to temporarily restrict access to certain sites during a certain time of day :)

Sets the start time (start_time) and end time (finish_time) to block access to specific sites. In this case, access will be limited from 9:00 to 20:15 every day.
Creates a path to a 'hosts' file on a Windows system that contains information about which sites should be redirected to.
Specifies the URL ('127.0.0.1') to which access will be redirected.
Creates a list of blocked sites.

In an infinite loop, checks the current time. If it is between start_time and finish_time, then access to blocked sites is limited by adding them to the 'hosts' file. If the current time falls outside this interval, then all lines that relate to blocked sites are deleted from the 'hosts' file.
After each check and processing of the 'hosts' file, the program stops for 5 seconds before the next check.
