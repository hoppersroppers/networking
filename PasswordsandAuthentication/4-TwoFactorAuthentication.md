# Two Factor Authentication

<iframe allowfullscreen height="360" src="https://www.youtube.com/embed/QrlEmfDu0OM?wmode=opaque" width="640"></iframe>  

You've probably seen two-factor authentication before (aka those
annoying texts and emails), but let's go a bit into the theory. 

Read this: <a
href="https://www.cs.cornell.edu/courses/cs513/2005fa/NNLauthPeople.html"
rel="noopener"
target="_blank">https://www.cs.cornell.edu/courses/cs513/2005fa/NNLauthPeople.html</a>

A brief note: Cell phone text messages aka SMS are commonly used for
multifactor auth. These are not great, because a)
<a href="https://www.wired.com/story/sim-swap-attack-defend-phone/"
rel="noopener" target="_blank">someone can steal your phone number and
get the texts sent to them</a> b) <a
href="https://www.theguardian.com/technology/2016/apr/19/ss7-hack-explained-mobile-phone-vulnerability-snooping-texts-calls"
rel="noopener" target="_blank">intercept your text messages</a>

However, those things are not in your threat model unless you are famous
or have cryptocurrency wallets. So don't worry about it, SMS 2FA is
great.

Another note: Just because you have multi-factor doesn't mean you can't
get phished for it!
