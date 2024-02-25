# Firewalls, Port-Forwarding, and iptables

<iframe allowfullscreen height="360" src="https://www.youtube.com/embed/yiItNwKbzQo?wmode=opaque" width="640"></iframe>  

Alright, time for some hacker stuff. 

I'm not going to get too deep into this, but I am going to give you
enough of a vibe of what is going on that you will appreciate how much
complexity exists here. 

First, let's talk iptables.

### iptables

According to the manpage, *"Iptables and ip6tables are used to set up,
maintain,  and inspect the  
tables of IPv4 and IPv6 packet filter rules in the Linux kernel.
 Several different tables may be defined.  Each table contains a number
of built-in chains and may also contain user-defined chains.  
  
Each chain is a list of rules which can match a set of packets.  Each
rule specifies what to do with a packet that matches.  This is called a
\`target',  which may be a jump to a user-defined chain in the same
table."*

Okay so what does that mean? Basically, iptables are a rules-based
system for controlling the flow of network traffic, and basically, every
Linux system has it. This means that we can create routing rules to do
almost anything we want from the command line.

#### iptables as a Firewall

Firewalls are similarly rules-based systems, but you probably think of
them as some big system that keeps hackers out of a giant network, not
just a single box. But a dirty secret of those expensive firewalls is
that many of them rely on iptables under the hood. Let's play around
with a couple one-liners to show the power. (and yeah, you'll need root)

  

First, run $ iptables -L to see what rules are already configured. Most
likely you are currently set up to accept all INPUTs, OUTPUTs, and
FORWARDs by default. That's fine, but it's also fine if you've got some
other rules going on. Docker and plenty of other programs set up their
own iptables rules. 

  

So let's say we have a sensitive service running on port 1337 we don't
want anyone to get access to.

Let's add an iptables rule:

$ iptables -A INPUT -p tcp --dport 1337 -j DROP

Now when you run $ iptables -L you should see the rule 

Chain INPUT (policy ACCEPT)  
target     prot opt source               destination          
DROP       tcp  --  anywhere             anywhere             tcp
dpt:1337  
  
Good luck connecting to that now! Try with netcat.  
  
Now to turn that rule off we can use $ sudo iptables -L --line-numbers
which will give us a number in front of the rule (in this case 1)

We can use that, coupled with the INPUT Chain name, to run $ sudo
iptables -D INPUT 1 to delete the rule. Using -L will show that the rule
is gone again. 

There are infinite iptables resources out there, but this is a good
start.

###  

### iptables for port forwarding

I was going to write up a quick tutorial on this, but hey, you're an
adult, just read a StackOverflow response like the rest of us real
hackers. The goal here is to nc to one local port and connect to a nc
listener on a different local port.

[SO: How to Do Local Port
Forwarding](https://stackoverflow.com/questions/28170004/how-to-do-local-port-forwarding-with-iptables)

  

For this assignment, submit anything you found difficult to understand
and try to talk through it. Don't spend too much time on the assignment,
the experimentation is the goal.
