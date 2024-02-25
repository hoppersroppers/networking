# Threat Modeling

<iframe allowfullscreen height="360" src="https://www.youtube.com/embed/RAl-pkdwOSg?wmode=opaque" width="640"></iframe>  

Read this, it's a pretty entertaining writeup: <a
href="https://arstechnica.com/information-technology/2017/07/how-i-learned-to-stop-worrying-mostly-and-love-my-threat-model/"
rel="noopener" target="_blank">Sean Gallagher: How I Learned to Stop
Worrying and Love my Threat Model</a>. I got lunch with the author once
and he was a super good guy. 

<img
src="https://files.cdn.thinkific.com/file_uploads/429463/images/d5b/43d/432/1642440354881.jpg"
class="fr-dib"
srcset="https://files.cdn.thinkific.com/file_uploads/429463/images/d5b/43d/432/1642440354881.jpg?width=1920 1x, https://files.cdn.thinkific.com/file_uploads/429463/images/d5b/43d/432/1642440354881.jpg?width=1920&amp;dpr=2 2x, https://files.cdn.thinkific.com/file_uploads/429463/images/d5b/43d/432/1642440354881.jpg?width=1920&amp;dpr=3 3x"
style="width: 300px;" />

Use this page from the good guys at the EFF to help assess what your
risks are: <a href="https://ssd.eff.org/en/module/assessing-your-risks"
rel="noopener"
target="_blank">https://ssd.eff.org/en/module/assessing-your-risks</a>

What do you want to protect? Who do you want to protect it from? How
likely is it that you will need to protect it? How bad are the
consequences if you fail? How much trouble are you willing to go through
in order to try to prevent those?

1.  For this exercise, our list of things we are trying to protect will
    be your email account and your phone's photos.
2.  For each, write down where it’s kept, who has access to it, and what
    stops others from accessing it.
    -   Do this on paper, not electronically.
3.  Think of three possible threat actors who might want to get a hold
    of your data or communications. It might be an individual, a
    government agency, or a corporation.
    -   As an important note, you are significantly more likely to be
        "hacked" by someone you know than some random internet stranger.
        This is even more likely to occur with significant others or
        parents who you may not normally consider adversaries.
4.  Think about what each adversary might want to do with your private
    data
5.  Think about what the likelihood of each adversary coming for that
    data
6.  Think about what happens to you if the adversary gets that data
7.  Now try to answer the question, how much trouble are you willing to
    go through in order to prevent loss.
8.  Think about if you had typed this information rather than written it
    on paper
9.  What would it take for a hostile entity to capture what you just
    wrote down if it was:
    -   On a piece of paper
    -   A local word document
    -   A google doc

Now destroy the paper you just wrote on. Or don't. Decide how much risk
you incur by keeping it.

<img
src="https://files.cdn.thinkific.com/file_uploads/429463/images/706/0ec/17a/1642440464339.jpg"
class="fr-dib"
srcset="https://files.cdn.thinkific.com/file_uploads/429463/images/706/0ec/17a/1642440464339.jpg?width=1920 1x, https://files.cdn.thinkific.com/file_uploads/429463/images/706/0ec/17a/1642440464339.jpg?width=1920&amp;dpr=2 2x, https://files.cdn.thinkific.com/file_uploads/429463/images/706/0ec/17a/1642440464339.jpg?width=1920&amp;dpr=3 3x"
style="width: 300px;" />

One important note is that you might not have anything worth a targeted
attack personally, but you have access to other things that might be
interesting to other people. For example, your contact lists can be used
to identify other, more important targets. Even more dangerous, someone
could use your account to send phishes to your contacts. A @navy.mil
address is going to have a significantly higher click rate than some
random @gmail. You also have access to your network, so someone could
use you to pivot to a network you have access to.

Submit any feedback you have on this threat modeling activity.
