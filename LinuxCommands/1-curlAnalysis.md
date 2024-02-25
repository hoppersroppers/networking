# curl Analysis

<iframe allowfullscreen height="360" src="https://www.youtube.com/embed/dvWNeEcs96c?wmode=opaque" width="640"></iframe>  

Read this to learn about how making a web request works: [Mozilla: How
the Web
Works](https://developer.mozilla.org/en-US/docs/Learn/Getting_started_with_the_web/How_the_Web_works)

Too bad all the web traffic is encrypted these days with HTTPs, that's
super boring. Guess we'll have to go and find a HTTP website to look at
for now, but for now, instead of using a web browser, we'll use a
command line tool.

There are plenty of tools to download a file from the terminal, but I
prefer to teach curl as it is able to support the most protocols (and
can upload too if you need it). 

Steps:

1.  ``` default
    Begin capturing packets in Wireshark on the correct external interface
    ```

2.  `Run the command ``$ curl  http://httpforever.com/`

3.  `Run the command: ``$ wget http://httpforever.com/`

4.  Stop your capture.

`Assignment:`

1.  `Can you find a DNS request to httpforever.com? What is the filter needed to find it?`
2.  `What is the port you hit the site on?`
3.  `What is the default HTTP port?`
4.  `What happened when the connection started?`
5.  What filter is needed to see all traffic between the site and you?
6.  What did you see if you follow TCP stream?
7.  Were you able to see anything? If you did, can you extract the
    file(s)?
8.  What is the difference between the UserAgents in the two requests?
    Why?
9.  What happened when the connection ended?
10. Was there anything else you found interesting? 

Submit a text file?
