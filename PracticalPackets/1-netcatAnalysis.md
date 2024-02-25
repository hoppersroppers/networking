# netcat Analysis

<iframe allowfullscreen height="360" src="https://www.youtube.com/embed/xRc74ovxSYs?wmode=opaque" width="640"></iframe>  

Netcat is known as the "Swiss Army Knife" of networking tools. Whatever
you want to do, you can probably do it with netcat. It comes
pre-installed on most Linux machines, which makes it a common
troubleshooting tool. While there are many features, the most common use
is that you can use it to send and receive arbitrary data across a
network. The way we send data across a network is with things named
"protocols". Netcat speaks the TCP and UDP protocols, but that doesn't
matter all that much right now. Protocols run everything online, but we
are going to save learning how they work for later. 

For this lab, you are going to play around with Wireshark and sockets.
Don't rush through it, take your time and experiment.

1.  Begin capturing packets in Wireshark on the correct interface. In
    this case, that means the local "lo" interface, rather than your
    external one. 'Any' works as well. 

Using pipes and redirectors that we learned about in the last lesson, we
can choose the input that is sent via the network, as well as what we do
with the data once we receive them. On the command line we can use `nc`
as a short name for the netcat program.

``` default
$ echo 'Hello World' | nc 127.0.0.1 1337
```

When we run this first commnd, we take the STDOUT of echo and pipe it as
the STDIN of netcat. The first argument for netcat is the IP address we
want to send it to, and the second number is the port we want to send it
to. Netcat will then send 'Hello World' off to the correct location.
Networking is hard, but we will skip a lot of the hard stuff for now. At
this time, just know that most computers have an IP address and have
thousands of ports. If two computers want to pass data over a network,
they have to know the correct IP address and port to send data to.

In this case, we are using netcat to send 'Hello World' to IP address
127.0.0.1 to port 1337. IP address 127.0.0.1 is often known as
localhost, and is our current computer. You can also write that command
as:

``` default
$ echo 'Hello World' | nc localhost 1337
```

If you noticed, nothing happened on the command line, which is kind of
expected. 

*What happened in Wireshark when you ran the command? Was there some
sort of error? Can you see any data?*

What happened was we tried to send without setting up something to
listen! Now we get to see what netcat can really do! Open up a new
terminal and set up a listener on localhost port 1337 with this command.

``` default
$ nc -l 1337
```

Now you have set up a listener, go and run the first command again from
your other terminal to send 'Hello World'.

*Check it out in Wireshark again! What happened this time?!*

Look at that! You have NETWORKED!!!!! To stop listening, press ctrl-c.
That generally closes out or "interrupts" most processes in the
terminal.

Let's talk about what just happened. First, you set up a "server", the
listener. Then you had the "client" send data to the listener. This is
about the most basic client-server setup you can get, but the principles
remain generally the same all the way up to the complexity of web pages.

## Send a File

For more fun, we can even send files around using redirectors because of
how well Linux handles streams.

First modify your listener to output to a file using '\>'. Then, use
`cat` to read an existing file into a stream and then use '\|' to pass
it into netcat. This might require some fiddling for you to get the
streams lined up properly. If needed, use Wireshark to make sure things
are being sent.

Eventually it should work, and you should have transported the file into
the new location where your listener was pointing!

*What's even cooler is that you should be able to use Wireshark to pull
that data out of the packets!*

Alright, so that wasn't magic, though it is pretty cool. 

##  

Assignment:

1\. Submit what you learned from this section. Don't spend too much time
on the writeup, I want you to focus on experimenting.
