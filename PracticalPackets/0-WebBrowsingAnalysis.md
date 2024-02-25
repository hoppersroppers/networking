# Web Browsing Analysis

<iframe allowfullscreen height="360" src="https://www.youtube.com/embed/qQlratM7VHo?wmode=opaque" width="640"></iframe>  

Time to get after it and start looking at things! This is where the
rubber meets the road.

Start recording packets in Wireshark! Make sure to choose the correct
interface. Interfaces are tricky, but basically look for the one
probably starting with en or wl with a bunch of traffic. At least in
this case! 

Depending on what you are trying to capture you have to change
interfaces... "lo" or loopback,  is your local interface for packets
that never leave your box (which is important for local testing, but not
the right place to look for traffic going externally. 

With Wireshark fired up, you should see all sorts of traffic stacking up
in there, probably with a ton of protocols you've never heard of. 

For now, visit [roppers.org](//roppers.org) and then end your session. 

Assignment:

1.  What filter was required to only see [Roppers.org](//Roppers.org)
    traffic?
2.  What protocol was used?
3.  What port was used? 
4.  Were you able to see any information in the browsing session? 
5.  Why not?
6.  Was there anything else that interested you?

Damn HTTPs makes sniffing web traffic boring! At least it's secure these
days!
