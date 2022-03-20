# Hostile Networks Intro
##  [Register for the Free Course Today!](https://www.roppers.org/courses/security)
## Intro
Add this to the list of security truisms.

"Any network connected to the internet must be considered hostile." Most intranets should be considered hostile too. 

But what does "hostile" mean? In this case, the general idea is that if computer A wishes to communicate with computer C, that means that they need to send all of their traffic through computer B. Gentlemen's agreements not to look at that traffic might have worked on Arpanet, but not anymore.

From Internet Service Providers (ISPs) working with governments to snoop on all your traffic, to deep sea submarine cable intercepts to sketchy free wifi hotspots, your internet browsing is recorded by a lot of people. And when I mean, a lot of people, I mean literally every single hop on your way across the internet (remember traceroute?) will have a complete log of your connections. They might not have the content if you have encrypted your traffic, but they will have records of the date/time the request was made, from who, and to where. This is accesssible to anyone with access to the logs, whether they own it, pwned it, or have a court order. Your IP address is likely shared, but if logs are kept all the way down, and they likely do exist, anything can be tracked down to you.

This next section skips over the technical details of network ownage (while giving you plenty to research on your own time), and focuses on the principles that can protect you and specific steps you can take to protect yourself.


# Why Network Security Matters

First, let's get into threat modeling... If you are doing something so 'fun' that if someone was able to provably demonstrate that you were the one behind the keyboard at the time you would go to jail or worse, this is the most important of all the sections. But you hopefully don't fall into this category, and more likely are worried about online censorship, aka web content filters. That's how I started. 

So while we mostly care about circumventing censorship, we will also teach as if you had to care about bad guys getting your IP address. 

It's a good thing to know.