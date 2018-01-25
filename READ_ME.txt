SBP and SLP .zip files are exports of two NetBeans projects - server/client

 - SBP is written in C - it is compiled in C11 standard and it is using -D_POSIX_SOURCE parameters
 - SLP is writen in C++ - it is compiled in C++ 11 standard and is using -lboost_system -pthread parameters


The projects are set-up to use a remote build host shellsrv.dcs.aber.ac.uk
There is one hard-coded file  and it is wagons-data.txt it is used by SLP and is located in the SLP folder.
The server and the port are hard-coded as well.


the SBP accepts five commands:
 - config command - allocate/reallocate memory for sidings e.g. config 5 5 4 4 3 3
 - load command - populate the sidings with wagons e.g. 0 3 2 1 2 1
 - move command - moves a number of wagons from siding A to siding B using the headshunt e.g. 1 2 3 
 - client exit command - quit
 - both server and client exit command - ]!


dpv_CS23820_report.pdf is the report required by this assignment.
dpv_SCREEN_CAST.flv is the screencast required by this assignment.