Are you a power-user with 5 minutes to spare? Do you want a faster internet experience?

Try out namebench. It hunts down the fastest http://en.wikipedia.org/wiki/Domain_Name_System'>DNS servers available for your computer to use. namebench runs a fair and thorough benchmark using your web browser history, tcpdump output, or standardized datasets in order to provide an individualized recommendation. namebench is completely free and does not modify your system in any way. This project began as a 20% project at Google.

namebench runs on Mac OS X, Windows, and UNIX, and is available with a graphical user interface as well as a command-line interface.
http://namebench.googlecode.com/files/screenshot-1.3.png'>
namebench was written using open-source tools and libraries such as http://www.python.org/'>Python, http://wiki.python.org/moin/TkInter'>Tkinter, http://pyobjc.sourceforge.net/'>PyObjC, http://www.dnspython.org/'>dnspython, http://jinja.pocoo.org/2/'>jinja2 and http://graphy.googlecode.com/'>graphy.


Screenshots
Here is what the nameserver overview looks like:

http://namebench.googlecode.com/files/screenshot-1.3-table.jpg'>

Here are what some of the graphs produced look like:

http://namebench.googlecode.com/files/screenshot-1.3-graphs.jpg'>

Command-line version
If you are running the command-line version, you get something that looks like this:



Final list of nameservers considered:


------------------------------------------------------------------------------


130.85.1.5      UMBC 5 US          56  ms | 


208.67.222.220  OpenDNS-3          56  ms | www.google.com is hijacked: google.navigation.opendns.com


209.244.0.4     Level3-R2          62  ms | 


216.146.35.35   DynGuide           63  ms | NXDOMAIN Hijacking


204.9.56.9      BroadAspect US     63  ms | 


8.8.4.4         Google Public DNS- 64  ms | Replica of Google Public DNS [8.8.8.8]


208.67.220.220  OpenDNS            65  ms | www.google.com is hijacked: google.navigation.opendns.com


156.154.70.1    UltraDNS           67  ms | NXDOMAIN Hijacking


127.0.0.1       Localhost IPv4     68  ms | NXDOMAIN Hijacking (www)


209.18.47.61    RoadRunner NC US   68  ms | Replica of RoadRunner NC-2 US [209.18.47.62], NXDOMAIN Hijacking (www)


156.154.71.22   Comodo Secure DNS- 80  ms | NXDOMAIN Hijacking


209.18.47.62    RoadRunner NC-2 US 104 ms | (excluded: Slower replica of RoadRunner NC US [209.18.47.61])





- Sending 250 queries to 11 servers...





Mean response (in milliseconds):


--------------------------------


Google Public DN ################# 64.85


Comodo Secure DN ################### 72.84


RoadRunner NC US ####################### 91.19


UltraDNS         ####################### 91.61


Localhost IPv4   ########################### 108.66


OpenDNS          ############################ 110.69


OpenDNS-3        ###################################### 149.85


DynGuide         ####################################### 156.60


Level3-R2        ########################################### 169.81


UMBC 5 US        ########################################### 172.63


BroadAspect US   ##################################################### 214.19





Response Distribution Chart URL (200ms):


----------------------------------------


http://chart.apis.google.com/chart?cht=lxy&chs=720x415&chxt=x,y&chg=10,20&chxr=0,0,200|1,0,100&chd=t:0,8,8,9,10,1...





Response Distribution Chart URL (Full):


---------------------------------------


http://chart.apis.google.com/chart?cht=lxy&chs=720x415&chxt=x,y&chg=10,20&chxr=0,0,3500|1,0,100&chd=t:0,0,0,1,1,1...





Recommended configuration (fastest + nearest):


----------------------------------------------


nameserver 8.8.4.4         # Google Public DNS-2  


nameserver 127.0.0.1       # Localhost IPv4  


nameserver 209.18.47.62    # RoadRunner NC-2 US