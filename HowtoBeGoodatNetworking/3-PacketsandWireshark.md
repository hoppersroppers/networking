# Packets and Wireshark

<iframe allowfullscreen height="360" src="https://www.youtube.com/embed/yyy-NLFsm7I?wmode=opaque" width="640"></iframe>  

Remember when I said that RFCs are the specifications and thus, are the
ground truth? I lied. 

Humans implement the specs, and humans are fallible. Physics always has
a say as well. Which means that your packets can do whatever they want,
and there is a decent chance that they will. When that happens, the only
way to go is to get to the truth, and the ground truth is the content of
the encapsulated packets. 

First, we have to learn what a packet capture is. A packet capture is
the recording of all information that goes across your network. It is
possible to record all information that crosses a specific point in the
path and then play it back so that you can see everything that happened.
Plus you can look at the content of the encapsulated packets, which
means you can look for things that are going wrong. Packet captures
usually have the file extension .pcap or .pcapng, and are primarily
opened with a tool named Wireshark.

To look at packet content, we use Wireshark, a badass tool that has
existed for quite a while now. Wireshark is an amazing tool, install it
in both your native Windows and your VM. 

  

To start learning it we will use TryHackMe's module:

-   [Wireshark the
    Basics](https://tryhackme.com/room/wiresharkthebasics) - Learn the
    basics of Wireshark and how to analyse protocols and PCAPs

Complete that. 
