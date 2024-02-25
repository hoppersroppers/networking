# Python Simple HTTP Server and Requests

<iframe allowfullscreen height="360" src="https://www.youtube.com/embed/9gcFKd2Yjb4?wmode=opaque" width="640"></iframe>  

Every once in a while you need to distribute files to a group of people
on a local network or host a webpage, and you think, well, how am I
going to do that?

  

### Simple Server

Python, because they are thoughtful and caring and want us to be happy,
comes with a simple HTTP server by default, which we can stand up in
seconds. It used to be called SimpleHTTPServer in Python2, but now it
is:

$python3 -m http.server 

This will stand up a server that hosts the directory (and all other
files under that directory) that you ran the command in. Pretty awesome,
super convenient, and somewhat of a security risk (on your local
network) if you run it too high in your directory structure and share
too many files.

In your browser, go to the ip address and port it is running on and look
at the files being served! You are able to download whatever you need.

### Requests Library

Now of course, clicking around in a browser isn't hardcore enough for
us. Sure, we could use curl or wget to grab it from the CLI, but let's
say we want to do some python scripting. 

Now it is time for one of my favorite libraries, requests. It's an
elegant library that lets you do whatever you want to do with HTTP (and
HTTPS if you wrap it). Use [these
docs ](https://docs.python-requests.org/en/latest/)to write a short
script that can grab all the files on your local server and save them. 

For your assignment, submit the script.

  
