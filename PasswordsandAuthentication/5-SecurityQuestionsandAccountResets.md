# Security Questions and Account Resets

<iframe allowfullscreen height="360" src="https://www.youtube.com/embed/DjKA5TBJ_0E?wmode=opaque" width="640"></iframe>  

What is your mother’s maiden name? First dog? Elementary school? All of
those things are fairly easy to find online, or just from casual
conversation. If someone is trying to steal an account, that will always
be the easiest route. Security questions are hard to avoid, but there
are easy ways to harden yourself and protect your accounts.

Read this: <a
href="https://www.wired.com/2016/09/time-kill-security-questions-answer-lies/"
rel="noopener"
target="_blank">https://www.wired.com/2016/09/time-kill-security-questions-answer-lies/</a>

Luckily, there is a better way. Instead of forcing you to lie, we are
going to introduce you to the ideas of hashing and salting.

### Hashing and Salting

Combining the ideas of salting and hashing, now learn how you are going
to make secure security questions! First, as a rule, don't use uppercase
letters, spaces, or punctuation ever in your security questions. Why?
Nothing about security, it just makes them easier to remember, and if
they are long enough, it won't be brute-forceable. Then if we take a
hashing algorithm, like MD5, and a unique salt you reuse across sites,
such as “salty17”, we can use the pseudo-function
MD5(*answer_to_question* + “salty17”). This will create a very very hard
to figure out security question that you can easily use anywhere. To
make it easier on yourself, maybe just take the first 10 characters from
the hash.

Or, if you are on a computer with your password manager, just write it
down in your secure notes for a site. If they get your LastPass account
you are not doing well anyway, so don't worry about it.

Submit the first 10 characters of the MD5 hash of "fido" + "salty17".
