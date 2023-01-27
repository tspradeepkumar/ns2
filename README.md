# ns2
TCL Scripts related to NS2

Copy the files (wired.tcl) and telnet.awk in the same folder and run the wired.tcl using the following command. 

$ns wired.tcl 
The above file shows the demo of a FTP and Telnet Application and later the throughput can be measured using the AWK script. The above command generates two files namely out.tr and out.nam. 
You can see the nam window of 5 nodes that exchange the FTP and Telnet app. 
To see the throughput calculation, use the following command

$ gawk -f telnet.awk out.tr 

This line will print two lines shows the throughput of FTP and Telnet.
