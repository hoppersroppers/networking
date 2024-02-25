# Don't Get Hacked

<iframe allowfullscreen height="360" src="https://www.youtube.com/embed/2jaB59dYJ3k?wmode=opaque" width="640"></iframe>  

Simple, right?

Alright so your computer is clean, probably, after following the last
steps, now if you get infected in the future the most likely scenario is
that you ran someone else's code and gave them access to your computer.
There's nothing to feel bad about, this could have happened in many
ways, and it happens to the best of us. Common ways this could have
occured are online installers, phishing, and downloaded tools getting a
malicious update. We will go over each method, and how to avoid it in
the future.

## Downloading Nasty Stuff

Downloading something nasty is the easiest way to do this, whether it is
from an email, a big green download arrow on a website, or a program
from a torrent site. Phishing is the most common, because it is the most
targeted, which results in a higher install rate. We talked about this
earlier in the Passwords section, so not much has changed, except the
goal is for you to install a program or open a file, rather than type in
credentials.

Now what do you do if someone tries to phish you, or you are wondering
if this is a phishing attempt? Read this: <a
href="https://decentsecurity.com/malware-web-and-phishing-investigation/"
rel="noopener"
target="_blank">https://decentsecurity.com/malware-web-and-phishing-investigation/</a>

If you get a phish, good chance other people are getting it as well. So
you need to report it! Make sure you know how to report to your
organization to protect everyone else!

You could have also run some backdoored file, whether from an online
download, or packaged in with real software. A good move before
downloading anything is run it through these sites listed in the
anti-phishing tools. These sites are pretty awesome and use a lot of
cool technology to make a determination if something is malicious.

Attachment and file checkers use something called a "sandbox" to open
the file/execute the program. The sandbox monitors the process created
and looks for any malicious behavior, in addition to running anti-virus
looking for a known bad.

URL checkers use a browser to visit the URL and look for malicious
behavior, like attempts at infection using an exploit. They also usually
provide historical information about the website and if it has been used
to host malware before.

IP Checkers look at historical data for an IP address or block of IP
addresses to see if they have been used for shady things in the past.
Remember the difference between and IP and a URL?

Tasks:

1.  Write a few sentences on why a URL could be clean historically but
    the IP address could be bad. This is going to require your
    understanding of hosting servers and domain names.
2.  Analyze a malicious attachment
    (https://github.com/heptastique/infected-pdf) using a few of the
    sites. Write about some of the data it provides and what you can do
    with it. This is an old, but very much live piece of malware. If you
    download this to a computer with active anti-virus, it will be
    blocked. I strongly recommend downloading it to Linux and not
    opening it up, even though your pdf reader is patched by this point.
    Just good habits.
    -   <a href="https://app.any.run/" rel="noopener"
        target="_blank">https://app.any.run/</a>
    -   <a href="https://www.virustotal.com/gui/home/upload" rel="noopener"
        target="_blank">https://www.virustotal.com/gui/home/upload</a>
