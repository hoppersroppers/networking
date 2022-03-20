# Windows Network Threat Hunting  
##  [Register for the Free Course Today!](https://www.roppers.org/courses/security)
Network hunting on Windows is basically the same thing as on Linux, it's all just packets. Packet captures from all operating systems will be saved in the same place on the security monitoring server and network analysts will look at them using the same tools. Even looking at Wireshark captures locally will be basically the same, though there will be a bunch of weird looking Microsoft protocols going on that all look like malware C2 but really are benign. "Know normal, find evil", so get used to the weirdness.

The primary difference for you will be what tools you use to look for rouge local connections. I recommend the built-in commands ```netstat ?ano``` and ```netstat ?af``` for that on Windows. 

Even better, an awesome Windows program named Glasswire identifies processes making network connections and alerts on them. If the process doesn't make sense when it pops up, go to Wireshark and open up the stream. 

Basically a self-sufficient threat hunter now.

### Glasswire Directed Hunt

1. Download Glasswire for Windows [https://www.glasswire.com/](https://www.glasswire.com/)
2. You already should have Wireshark downloaded. If not, download it.
3. Look at the Glasswire alerts. 
4. Choose one of the alerts for something that isn't a web browser and identify the stream in Wireshark.
5. Submit a description of what data was being sent and to whom based on your analysis.

### Undirected Hunt

Let's go boil that ocean!

0. Ensure all web browsers are closed
1. Open Wireshark and begin capturing traffic
2. After 30 minutes, work through packet capture, looking at what has the highest packet counts in "Statistics"
3. Trace the streams and identify what was going on.
4. Submit a brief explanation of what the top source of network traffic was during this time.