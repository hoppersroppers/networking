# Securing Linux According to Dennis
As mentioned earlier, there's basically no malware for Linux. Why, well it really comes down to market incentives. There aren't many people running Linux machines, and of those, few of them are desktop users. So compromising those few desktop users so that an attacker can steal browser credentials and banking information just doesn't make much sense to the criminals of the world. (Not to mention, people who are using a free operating system can't have that much money to steal, amirite?)

The vast majority of Linux malware is targeted towards servers, routers, etc, and mostly meant to get access into Windows networks that lie inside the DMZ. As you are running Linux in a VM most likely, or at worst as your regular host machine, these threats are of minimal importance to you. 

[<img src="https://imgs.xkcd.com/comics/linux_user_at_best_buy.png
">](https://xkcd.com/272/)

So would I be a bad person if I told you your default build of whatever Linux OS you are using is good enough? Maybe, maybe not. Check your threat model. I don't harden my local Linux boxes at all, and if I did need a hardened box, I'd be using Qubes, not a "hardened" Ubuntu build. 

The only change I recommend (and even then, not all that strongly) is setting up [automatic unattended upgrades](https://www.cyberciti.biz/faq/set-up-automatic-unattended-updates-for-ubuntu-20-04/). If you are not on Ubuntu-20.04 you'll have to find another guide. 

If you still want to look for more ways to harden Linux, [check out this link](http://cypat.guru/index.php/Linux_Hardening). I just don't think you need to do it, but at least it is interesting. 