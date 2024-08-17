# telnet Analysis

## <iframe allowfullscreen height="360" src="https://www.youtube.com/embed/Q2hjh3kk2jE?wmode=opaque" width="640"></iframe> 

## Telnet

Telnet is an old fashioned protocol that usually provides nice and easy
shell access to anyone running a telnet server, which is often
unauthenticated. It's a hacker's dream!

Too bad you don't see many of them these days, but they are common in
CTFs, and on critical infrastructure (jokes?).

Here's a fun telnet demo to show what it is capable of:

``` default
$ telnet towel.blinkenlights.nl
```

Hackers gonna hack. And bored people... well they're gonna bored people.

Steps : 

1.  Begin capturing packets in Wireshark on the correct interface
2.  `Run the command: telnet towel.blinkenlights.nl`
3.  `Once connected, watch for a bit and then end the connection.`

`Assignment:`

1.  `What is the standard telnet port?`
2.  `What happened when the connection started? This might not work if your ISP is blocking telnet. If this didn't work, `[`bask in this glory.`](https://www.youtube.com/watch?v=Dgwyo6JNTDA)
3.  What filter is needed to see all traffic between the site and you?
4.  What did you see if you follow TCP stream?
5.  Were you able to see anything? 
6.  What are the different protocols that Wireshark dissects for you?
7.  What happened when the connection ended?
8.  Was there anything else you found interesting? 
