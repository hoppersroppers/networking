# OSI Model and Encapsulation

<iframe allowfullscreen height="360" src="https://www.youtube.com/embed/quGCqcNReNY?wmode=opaque" width="640"></iframe>  

The OSI Model (aka the Open Systems Interconnection model but you'll
never see that) is a useful mental model of how internet communications
system work and interact with each other.

Basically, the idea is that each level  of the model is a different part
of what is necessary for data to be transferred from one place to
another. We will learn all about it as we go, so don't worry about
memorizing anything... yet. 

<img
src="https://files.cdn.thinkific.com/file_uploads/429463/images/2cb/2de/750/1644638268259.jpg"
class="fr-dib"
srcset="https://files.cdn.thinkific.com/file_uploads/429463/images/2cb/2de/750/1644638268259.jpg?width=1920 1x, https://files.cdn.thinkific.com/file_uploads/429463/images/2cb/2de/750/1644638268259.jpg?width=1920&amp;dpr=2 2x, https://files.cdn.thinkific.com/file_uploads/429463/images/2cb/2de/750/1644638268259.jpg?width=1920&amp;dpr=3 3x"
style="width: 300px;" />

The competitor to OSI is the TCP/IP model, which is basically the same
thing, but with less layers. It all shows the same thing, just with
different levels of specificity. 

  

### Encapsulation

One useful thing we can use those models for is to visualize how
encapsulation works. Encapsulation is the process of wrapping a piece of
data in the routing information required to pass to the next level of
the networking stack. Once it gets to the bottom of the stack at the
physical layer and is actually sent across the network, once it is
received "de-encapsulation" occurs, and each level of encapsulation is
removed. Eventually, the data, as sent from the first computer finally
reaches its destination. 

<img
src="https://files.cdn.thinkific.com/file_uploads/429463/images/c09/a64/839/1644638396779.jpg"
class="fr-dib"
srcset="https://files.cdn.thinkific.com/file_uploads/429463/images/c09/a64/839/1644638396779.jpg?width=1920 1x, https://files.cdn.thinkific.com/file_uploads/429463/images/c09/a64/839/1644638396779.jpg?width=1920&amp;dpr=2 2x, https://files.cdn.thinkific.com/file_uploads/429463/images/c09/a64/839/1644638396779.jpg?width=1920&amp;dpr=3 3x"
style="width: 557px;" />

What does that mean? How does it work? Don't worry for now, you'll be
great at it soon enough.
