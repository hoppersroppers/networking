# You got Tricked

[Check out our free CTF Course!](https://academy.hoppersroppers.org/mod/page/view.php?id=924)

Alright so your computer is clean, probably, after following the last steps, now if you get infected in the future the most likely scenario is that you ran someone else's code and gave them access to your computer. There's nothing to feel bad about, this could have happened in many ways, and it happens to the best of us. Common ways this could have occured are online installers, phishing, and downloaded tools getting a malicious update. We will go over each method, and how to avoid it in the future. 


Downloaded Something Nasty

Downloading something nasty is the easiest way to do this, whether it is from an email, a big green download arrow on a website, or a program from a torrent site. Phishing is the most common, because it is the most targeted, which results in a higher install rate.

One of the biggest things you can do to avoid getting phished is to learn what a phishing attempt looks like. Read this: <https://blog.malwarebytes.com/101/2017/06/somethings-phishy-how-to-detect-phishing-attempts/>
Also, read this: <https://ssd.eff.org/en/module/how-avoid-phishing-attacks>

Now what do you do if someone tries to phish you, or you are wondering if this is a phishing attempt? Read this: <https://decentsecurity.com/malware-web-and-phishing-investigation/>

If you get a phish, good chance other people are getting it as well. So you need to report it! Make sure you know how to report to your organization to protect everyone else!

You could have also run some backdoored shit, whether from an online download, or packaged in with real software. A good move before downloading anything is run it through these sites listed in the anti-phishing tools. These sites are pretty awesome and use a lot of cool technology to make a determination if something is malicious. 

Attachment and file checkers use something called a "sandbox" to open the file/execute the program. The sandbox monitors the process created and looks for any malicious behavior, in addition to running anti-virus looking for a known bad. 

URL checkers use a browser to visit the URL and look for malicious behavior, like attempts at infection using an exploit. They also usually provide historical information about the website and if it has been used to host malware before.

IP Checkers look at historical data for an IP address or block of IP addresses to see if they have been used for shady things in the past. Remember the difference between and IP and a URL?

Tasks: 

1. Write a few sentences on why a URL could be clean historically but the IP address could be bad. This is going to require your understanding of hosting servers and domain names. 
2. Analyze a malicious attachment using a few of the sites. Write about some of the data it provides and what you can do with it.
3. Analyze a malicious program using a few of the sites. Write about some of the data it provides and what you can do with it.
4. Analyze a malicious URL using a few of the sites. Write about some of the data it provides and what you can do with it.
5. Analyze an IP using a few of the sites. Write about some of the data it provides and what you can do with it.
6. Read this: <https://www.digitalcitizen.life/uac-why-you-should-never-turn-it-off>. 
7. Turn UAC all the way up. Write what is UAC and why it protects you from malware.
8. How does malware bypass UAC, other than getting a human to enter the password? (Hint: Mitre Attack) There are a few answers, google around.
[Visit the course page!](https://academy.hoppersroppers.org/mod/assign/view.php?id=924)
