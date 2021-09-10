# MultiFactor Authentication
Read this: <https://www.cs.cornell.edu/courses/cs513/2005fa/NNLauthPeople.html>

Think about what multi-factor provides and what does it not provide?

Read through the options <https://www.lastpass.com/multifactor-authentication> and see what the different varieties are.

Check out this site to see all the things you can put multi-factor on. <https://twofactorauth.org/>

Read about how physical key devices work. <https://web.archive.org/web/20180422212245/https://www.yubico.com/why-yubico/how-yubikey-works/>. I used to have them, I don't anymore. Too inconvenient.

Read about [Google's Advanced Protection](https://landing.google.com/advancedprotection/). It is the best you can get right now but you probably don't need it. For the record, I don't use it. Too inconvenient.

A brief note: Cell phone text messages aka SMS are commonly used for multifactor auth. These are not great, because 
a) [someone can steal your phone number and get the texts sent to them](https://www.wired.com/story/sim-swap-attack-defend-phone/)
b) [intercept of text messages](https://www.theguardian.com/technology/2016/apr/19/ss7-hack-explained-mobile-phone-vulnerability-snooping-texts-calls)

However, those things are not in your threat model unless you are famous or have cryptocurrency wallets.

Another note: Just because you have multi-factor doesn't mean you can't get phished for it!