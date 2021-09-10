# Technical Attacks
In the last section, I discussed the idea of data minimization to avoid casual, non-technical invasions of privacy. But what about the uncommon attacks, done by someone who knows what they are doing? 

So let's say you work off a TrueCrypt partition with Full Disc Encryption. What risks remain?

## Rubber Hose Cryptography

Taking you and your computer and forcing you to give up password
* "Rubber hose cryptography"
   * <https://en.wikipedia.org/wiki/Rubber-hose_cryptanalysis> 
   * <https://xkcd.com/538/>
   * Some encryption tools allow the possibility of multiple partitions so that multiple passwords can be used. Only one password unlocks what you are actually trying to hide, others open different partitions, and there is no way of proving that there are multiple partition/password pairs... this doesn't work very well legally but might work. A little bit. 

There are plenty of legal issues surrounding forced password disclosure. In the US, there is more constitutional law in this field than you ever expected. Basically, US you are good, plead the 5th, self-incrimination. You'll still probably go down, but not for what is on the hard drive. Europe, you are going to jail. "Not chill" countries, beaten until you give it up, then jail.
	      
## Biometrics

If your device unlocks with anything on your body, they can just take you and open your stuff. Fingerprint/retina/voice/face unlocks are not protected by Constitution, they can just make you unlock these things if they have you. If you are in a "not chill" country, then doubly so.


## Tackling you off of the computer while logged in

Read this: ["They got DPR, they gonna find you"](https://www.businessinsider.com/the-arrest-of-silk-road-mastermind-ross-ulbricht-2015-1). They didn't need to tackle him, but they were very effective.

What if he had gotten the computer turned off? Read about [Cold Boot attacks](https://en.wikipedia.org/wiki/Cold_boot_attack).  While this sounds hard, I've done one before in a competition to recover FDE keys and it was actually pretty easy.

## Evil Maid and Black Bag Cryptanalysis

Black bagging can be used to describe an operation where you break into a physical location and do something for intelligence purposes. ALong those same lines, a physical attack on your computer, called an "Evil Maid", is a classic attack and near impossible to defeat. If you leave your computer alone for any period of time and a professional can tamper with it, you're going to be compromised.

Even with full disc encryption and a secure bootloader, if someone modifies the hardware and you use it, then you are still screwed. This can be throwing a new chip in your computer, throwing a keylogger in your keyboard firmware, or [really anything you can think of](http://www.nsaplayset.org/chuckwagon).

Read this: [F-Secure Evil Maid Guide](http://images.secure.f-secure.com/Web/FSecure/%7B319382b2-a040-4c88-bd94-20eed01bf22f%7D_F-Secure-Evil-Maid-Guide.pdf)

Where does an evil maid attack fall into your personal threat model? 
	    
It is also very possible to insert malicious hardware into a turned-on computer so.. turn them off when you leave the room, but really, if you're worried, bring them with you. 

	
## Electronic Emissions

It is possible for you to be surveilled by a local team based on your computer's hardware emanations! Is it likely? No! Is it cool! Yes!!!!

Read this: <https://en.wikipedia.org/wiki/Van_Eck_phreaking>
	
# Truecrypt Conspiracy Theory

Hey we are deep into threat modeling right now, read up on the [TrueCrypt Conspiracy Theory](https://nakedsecurity.sophos.com/2014/06/20/truecrypt-mystery-forking-weirder-than-before/). Who knows honestly, but it is interesting.

If someone has you and the computer, you are screwed. But more importantly, they had already found you, so you were already screwed.

Is there an answer to any of this? Not really, just risk model and move on.
