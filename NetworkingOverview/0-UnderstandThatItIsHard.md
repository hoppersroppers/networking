# Understand That It Is Hard

<iframe allowfullscreen height="360" src="https://www.youtube.com/embed/osuzRosdZtk?wmode=opaque" width="640"></iframe>  

Everything in computing is difficult, but networking is among the
hardest. The reason for this is fairly simple: More nodes external to
you means more complexity, especially because it adds complexity that
you do not control.

There are hundreds of ways why two computers can find themselves unable
to talk to eachother. Perhaps they are not turned on, or they aren't
plugged into the ethernet cord. Perhaps the ethernet cord is dropping
packets on the wire. Perhaps the wifi is getting interrupted. Perhaps
there is a firewall at the router that is blocking inbound connections.
Perhaps there is a firewall on the computer. Maybe the sockets aren't
open, or they are speaking different versions of the same protocol.
Maybe the protocol is fine but the application is buggy. Maybe the
application is working as intended but is configured to ignore these
connections, and you have to change the configuration. Maybe the Chinese
government is pretending to be the other computer and when you connect,
you are actually routing to them, but instead of Man-In-The-Middle-ing
you, they set up the script wrong and the operator who set it up is
being yelled at by his boss for messing up for the 5th time this week
and this time there is going to be formal paperwork and he just can't
keep bringing his personal problems into work and using it as an excuse
when he mistypes IP addresses.

So it is complicated.

On the plus side, networking is based on computers, and computers are
based on physics, which means we understand most of it. If something is
wrong with your networking, it's probably user error, at some stretch of
the line. Most of the time, it's your fault (Remember that). Sometimes
it is someone else's fault. That's when you can send an email and help
them fix it.

Very few things in networking are "undocumented". All of networking is
based around agreed upon standards from documents named RFCs. These
provide literally every piece of information required to send, receive,
and understand any protocol. Any time you are trying to understand a
protocol, the answer is in the RFC. That doesn't mean go straight to the
RFC, just like you shouldn't go straight to the man page. Wikipedia has
great intros to many common protocols, and always remember, you are not
the first person to run into a problem. Google is your friend, as
always.

Documentation only goes so far, sometimes you have to look at the ground
truth, which is the packets going over the wire.

Finally, DNS is always the problem.

Unless it's an old ethernet cable leaking packets (yes that is a thing
and good luck diagnosing that one).

This is a massive field, and nobody will ever be an expert in all of it.
You will however, become good enough to do whatever you need to do with
it, and that is all anybody asks of anyone on the internet.
