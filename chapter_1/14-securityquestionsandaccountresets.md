# Security Questions and Account Resets

[Check out our free CTF Course!](https://academy.hoppersroppers.org/mod/page/view.php?id=934)

What is your mother?s maiden name? First dog? Elementary school? All of those things are fairly easy to find online, or just from casual conversation. If someone is trying to steal an account, that will always be the easiest route. Security questions are hard to avoid, but there are easy ways to harden yourself and protect your accounts.
 
Tasks: 

* Read this: <https://www.wired.com/2016/09/time-kill-security-questions-answer-lies/>
* Submit what the article recommends you do

Luckily, there is a better way. Instead of forcing you to lie, we are going to introduce you to the ideas of hashing and salting.

### Hashing and Salting

Tasks:

* Read this: <https://crackstation.net/hashing-security.htm>. Not all of it, unless you really want to, just enough to answer these questions.
* In 2-3 sentences explain hashing and why it is important
* Describe each of the ways passwords are cracked
* In 2-3 sentences, explain what salting does and why it is important.

Combining the ideas of salting and hashing, now learn how you are going to make secure security questions! First, as a rule, don't use uppercase letters, spaces, or punctuation ever in your security questions. Why? Nothing about security, it just makes them easier to remember. Then if we take a hashing algorithm, like MD5, and a unique salt, such as ?salty17?, we can use the function MD5(_answer_to_question_ + ?salty17?). This will create a very very hard to figure out security question that you can easily use anywhere. 

Or, if you are on a computer with your password manager, just write that shit down in your secure notes for a site. If they get your lastpass account you are screwed anyway, so don't worry about it.
[Visit the course page!](https://academy.hoppersroppers.org/mod/assign/view.php?id=934)
