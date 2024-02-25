# SSH Analysis

<iframe allowfullscreen height="360" src="https://www.youtube.com/embed/tsLPNZjKw-M?wmode=opaque" width="640"></iframe>  

Another very important tool is Secure SHell or SSH. They are basically
the secure successor to Telnet for providing remote shells.

We won't go into the networking specifics of this yet, but SSH is a
networking protocol that allows encrypted access to remote computers.
How this works in effect is a remote computer, the SSH server, will
listen for an incoming connection. The local computer, which is the
client we are trying to SSH from, sends a request via the SSH protocol
to log in to the SSH server. If the password supplied is correct, the
server will then create a shell on the remote computer and then pass
back the stream from that shell to the client. From there, the client
who just logged in via SSH is able to have access to the remote computer
in an encrypted manner.

I hand waved a ton of complexity there, but it doesn't matter yet. We'll
spend some more time on this in the networking course, but you honestly
don't need to know the specifics, I certainly don't.

To SSH, you can either use a password or a key. Most of the time you
will have a password, and that is what we will focus on in this course.
The networking course will have more info on keys and SSH.

To use ssh, simply run the command: `ssh username@domain.com`. There are
plenty more options, but this one will get you through 90% of use cases.

Steps : 

1.  Begin capturing packets in Wireshark on the correct interface
2.  SSH into : `ssh bandit.labs.overthewire.org -p 2220 -l bandit0 w`ith
    the password `bandit0`
3.  `Once connected, get the first flag and then end your SSH connection.`

`Assignment:`

1.  `What port did you SSH into?`
2.  `What is the standard SSH port?`
3.  `What happened when the connection began?`
4.  What filter is needed to see all traffic between the site and you?
5.  Were you able to see the password? 
6.  Were you able to see anything? 
7.  What are the different protocols that Wireshark dissects for you?
8.  Was there anything else you found interesting? 

  

` `

  

  

  
