# Basics of Networking

<iframe allowfullscreen height="360" src="https://www.youtube.com/embed/JNfMYKopqQc?wmode=opaque" width="640"></iframe>  

I am going to handwave a bunch of things, just trust me, what I'm
handwaving doesn't matter that much for now. This is all part of some
kind of plan.

## IP Addresses and Basic Networking

You might have heard the word IP address before, but we aren't going to
dive too deep into it yet. Just think of it as the way other computers
know who you are, and based off of a complicated routing system, how
computers in between you and whatever you are talking to knows how to
transport things back and forth. There will be plenty more on this in
the Networking Course which you are going to do next anyway, so don't
worry about how it works.

To find out your IP address, run the command "ip addr". This will print
out a list of things called interface and some other stuff, don't worry
too much. For now, focus on the IP addresses, the items in the form
127.0.0.1, 192.168.20.45, 182.16.10.100, 10.2.5.24 etc.... addresses in
that form are known as IPV4 addresses. (There's another format known as
IPV6 that looks like but we aren't going to worry about them right now)

You should only have a few of them, so look for your 127.0.01 address.
This is called your localhost, aka, your computer's local IP address. It
is completely internal, and all computers have a localhost at 127.0.0.1.
This means that you can't talk to someone else's localhost address and
it is non-routable.

You should have at least one more IP address listed, likely in the
format 10.x.x.x, 192.168.x.x, or 172.x.x.x. These address ranges are
known as "local" addresses. Long story short, there aren't enough IPV4
addresses. If you want to read more about this,
<a href="https://en.wikipedia.org/wiki/IPv4_address_exhaustion"
rel="noopener" target="_blank">the wikipedia article</a> is decent.

To get around the lack of IPV4 addresses, most private networks use
these local addresses for all the computers on it, so that they don't
need to own all the IP address space required for all of their computers
(what? people own IP addresses? Yeah it's super complicated, we're gonna
ignore that for now. There's also something called IPv6 which looks like
this *2001:db8::8a2e:370:7334 *but we are going to ignore all of those
addresses for now)

So when you see those local IPV4 addresses, what you are seeing is the
IPV4 address your network has assigned to you to use locally (and only
locally).

## Routing

How do we connect to the internet then? Well, there's some magic called
routing we aren't going to worry about too much for now, other than to
be confident that it works.

Let's trace our route to google.com to confirm that routing is working
properly. In linux, this uses the command `traceroute`. Windows uses
`tracert`.

``` default
$ traceroute google.com
```

You should see a nice fancy print out of all the servers you've hopped
across, starting with your gateway router and ending with the google.com
server. This family of commands is especially useful for troubleshooting
networking problems.

(For a fun hack, try `traceroute bad.horse`. Gotta love abusing
protocols to do cool things)

So what does google see you as when you make a request?

I recommend a quick trip to a website to find that out!
<a href="https://nordvpn.com/what-is-my-ip/" rel="noopener"
target="_blank">Click here to find your public IP</a>.

As you can see, your public IP is completely different than what your
local IP is when you run `ip addr`.

The reason for that is something called NAT, or Network Address
Translation which is a method of mapping one IP address to another by
modifying packets while they are in transit. It's hella complicated how
it works, but what matters to us, the end users, is that our local
address is stored by some NAT server which ensures that any responses to
traffic from us that leaves our network, comes back to our locally
assigned IP. On the other hand, nobody should be able to connect into a
box behind NAT because they will not know the local IP address and
either way, a local address shouldn't be routed across the internet. So
just remember for now, NAT allows connections out and responses back,
but does not allow connections in. (Just smile and wave, nobody
understands NAT, but we'll go over it a bit more in the Networking
Course).

How does routing work? How do the packets actually get from Point A to
Point B? Patience my friend. Later in the course in the web section we
will talk about it.

## VM Networking

So how does this all tie back into practical application? Well your
Virtualization Software will have an option to switch your VM between a
NAT'd IP address and a Bridged IP address.

I don't spend much time on Windows in this course, but run the command
`ipconfig` in your Windows CMD prompt to get your host computer's IP
address.

Bridged IP addresses are IP addresses assigned by your local router,
which will be NAT'd by the router when you try to connect out. NAT'd IP
addresses are IP addresses assigned by your virtualization software,
which puts that box behind a NAT. This means that if you are NAT'd,
another local computer will not be able to connect to you, but if you
are Bridged, your IP address will be routable. You're still both behind
a router NAT, but it's the same NAT so you'll share the same IP address
prefix.

Depending on your Virtualization Software, switch between the different
networking modes and see how your IP address (and routing) changes. Run
the $ `ip addr` command to check. If you are having trouble switching,
assume that it is because Windows Hyper-V is doing bad things (even if
you aren't using it). It's possible to fix Hyper-V issues by "disable
network interfaces hyper-v" (there's your search term), but it's mostly
a pain that pops up every once in a while.

-   <a
    href="https://www.vmware.com/support/ws45/doc/network_configure_ws.html"
    rel="noopener" target="_blank">VMWare</a>
-   <a
    href="https://wiki.dave.eu/index.php/VirtualBox_Network_Configuration"
    rel="noopener" target="_blank">Virtual Box</a>
-   <a
    href="https://docs.microsoft.com/en-us/archive/blogs/virtual_pc_guy/using-hyper-v-with-a-wireless-network-adapter"
    rel="noopener" target="_blank">Hyper </a>V Don't try to do the
    HyperV one, it's a nightmare. Just install VMWare.

Over the next few sections and the rest of your life think about how
changes in your networking setup will effect routing.
