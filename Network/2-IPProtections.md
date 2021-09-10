# IP Protections
## Hiding Your IP and Circumventing Censorship


So now we know we need to add something in between ourselves and the things we are trying to visit. There are a varieties of ways to do that, but the most important bit is that we are able to trust the hops we are using, because a malicious hop is almost as bad as no hop at all. 

First, some vocab.

* Port forwarding = a network address translation technique where your router forwards incomming traffic to your computer, through a specific port.

* Proxy = an intermediary server between a packet's src and dst, designed to hide the ip of the src.

* Proxy chaining = connecting to multiple proxies betwwen src and dst.

* VPN = Virtual Private Network = a secure network connection between src and dst, operating as if there was a direct connection.

* TOR = The Onion Router = a network of nodes carrying traffic from the ToR browser, and encrypting traffic along the way. Designed to be a secure and anonymous web browser.

* Deep Web = The part of the Internet not indexed no search engines, but which is still accessible to the pubblic.

* Dark Web = The part of the Deep Web that is not accessible to the public. A VPN/ToRProxy/etc. is required.

       
## Circumventing Proxies and Going Right to the Source

Remember honey tokens and how we could use those? Or just regular malware. That calls home real nice. There's also a fine line in the middle referred to by some as a "Network Investigative Tool" which is basically just a system profiler that calls home and deletes itself.

## What Can Be Done with an IP

   * Identify general location 
   * DDOS their router 
   * Hack their Router
   * Court orders to ISPs
   * Threaten to give it to police so they can go get a court order

## Proxy

Now to add the proxy. Basically, this is a server you send a request to that routes all the traffic through them first, then passes it on to you. The critical thing to remember is that this extra hop added by the proxy, although it obfuscates your IP from the end target, does not hide it from the servers providing the proxy service. They can see all of your traffic and can do whatever they want with it. Your extra hops will create logs, and all those logs can still be used if someone gets them.
 
Visit <https://hide.me/en/proxy> and use their proxy to visit <http://www.whatsmyip.org/more-info-about-you/>.

Assignment:

1. How much information does What'sMyIP have about you compared to when you didn't use a proxy?
2. How much information does Hide.Me have about you now?

Adding an extra hop works, but it needs to be done intelligently, and certainly not through a sketchy website that provides it for free. Don't use free proxies, because if the product is free.... you are the product.