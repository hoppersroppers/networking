# traceroute Analysis

<iframe allowfullscreen height="360" src="https://www.youtube.com/embed/HO7OKh1-Smk?wmode=opaque" width="640"></iframe>  

Next you are going to learn about a really cool tool called traceroute. 

Steps:

1.  Ensure your VM Networking is set to Bridged
2.  Begin capturing packets in Wireshark on the correct external
    interface
3.  `Run the command ``$ traceroute hoppersroppers.org`
4.  Stop your capture and complete the first 5 questions.
5.  Change your VM Networking over to NAT
6.  Begin capturing packets in Wireshark on the correct external
    interface
7.  `Run the command ``$ traceroute hoppersroppers.org`
8.  When that fails, then run the command $ traceroute -I
    hoppersroppers.org
9.  Stop your capture and complete the rest of the questions.

`Assignment:`

1.  `What is Bridged Networking in a VM?`
2.  `What filter can you use to only see the traceroute packets?`
3.  `What happened when you ran traceroute?`
4.  What information can you see in the packets? What changes between
    each packet? 
5.  What happens with the TTL? How do you think traceroute works?
6.  What happened when the connection ended? Why?
7.  What is NAT? 
8.  What was the difference between the results from the last two runs
    of traceroute, and why? Check out [this
    link](https://superuser.com/questions/1582095/traceroute-does-not-work-properly-in-the-nat-mode-with-port-forwarding-in-virt)
    to learn what happens. 
9.  Was there anything else you found interesting? 

Submit a text file.
