# Scapy and Pwntools

<iframe allowfullscreen height="360" src="https://www.youtube.com/embed/HWyyxrJ4tzw?wmode=opaque" width="640"></iframe>  

Generating arbitrary packets and making connections is pretty easy in
Python, but what if.... they were even easier. Here we will introduce
two programs to make your life somehow, even easier.

  

### Scapy:

Scapy is a Python program that enables the user to send, sniff and
dissect and forge network packets. This capability allows construction
of tools that can probe, scan or attack networks.  
  
I will describe scapy as horrifyingly capable and ludicrously complex,
but it's way easier than a lot of other ways to generate arbitrary
packets and send them across the internet, so we'll call it a win. Check
out [the docs through the Quick
Demo](https://scapy.readthedocs.io/en/latest/introduction.html) to get
an idea of what Scapy is capable of. 

Experiment with this and look at what you are creating in Wireshark.

  

### Pwntools: 

pwntools is a CTF framework and exploit development library. Written in
Python, it is designed for rapid prototyping and development, and
intended to make exploit writing as simple as possible. Before we get to
exploits though, it provides a really great way to interact with
tubes... aka networking.

Work through the pwntools tutorials.

-   [Installing
    Pwntools](https://github.com/Gallopsled/pwntools-tutorial/blob/master/installing.md)
-   [Tubes](https://github.com/Gallopsled/pwntools-tutorial/blob/master/tubes.md)
    -   Basic Tubes
    -   Interactive Shells
    -   Processes
    -   Networking
    -   Secure Shell
    -   Serial Ports

If you want more practice using Pwntools, write a python script to solve
the first 5 challenges in Over the Wire Bandit.
<https://overthewire.org/wargames/bandit/>

(Hint:
<https://github.com/Gallopsled/pwntools-write-ups/blob/master/wargames/overthewire-vortex/level0/win.py>
)
