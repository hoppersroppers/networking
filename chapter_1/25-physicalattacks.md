# Physical Attacks

[Check out our free CTF Course!](https://academy.hoppersroppers.org/mod/page/view.php?id=947)

# Physical attacks

A physical attack on your computer, called an "Evil Maid", is a classic attack and near impossible to defeat. If someone has hands on keyboard after stealing your device, they own that computer unless you have protected it properly. If you have protected it properly and someone modifies the hardware, then you use it, then you are still screwed. If someone has you and the computer, you are screwed. Long story short, it is better for them to not know you are worth attacking, thus, OPSEC. However, sometimes you can't do that. Maybe you are a high profile individual who is in a hotel, maybe you live in a government dorm, maybe you are traveling and get border searched. This is the guide for those times. 

Tasks:

* Read this: <http://images.secure.f-secure.com/Web/FSecure/%7B319382b2-a040-4c88-bd94-20eed01bf22f%7D_F-Secure-Evil-Maid-Guide.pdf>
* Where does an evil maid attack fall into your personal threat model?

You can also mount an encrypted partition in your OS, and use that to hold a virtual machine to do your important work on. That gives you a ton of deniability, especially with the ability to make multiple partitions that unlock to different passwords. Remember though, if you get hacked on the outside, you get hacked in the VM as well. Either way, you need FDE and secure boot if you want to beat an evil maid.

Alright, now that you know that you need FDE and Secure Boot, lets go into various physical attacks on a computer and defenses against them.

1. Tackling you off of the computer while logged in
        * You can try a quick shutdown
	* Read about Cold Boot attacks
	    * <https://en.wikipedia.org/wiki/Cold_boot_attack>
	    * While this sounds hard, I've done one before in a controlled environment. Actually pretty easy.
	    
2. Breaking in to your hotel room and installing a keylogger, then breaking back in later and stealing your laptop now that they have the password. Or just arresting you.
        * <https://en.wikipedia.org/wiki/Black-bag_cryptanalysis>
	* Classic Boot attack
	* Installing keylogger
	
3. Malicious hardware to a turned on computer
	* USB Malware
	       * BAdusb
	       * Rubberducky
	       * BashBunny
	* FIREWIRE
	* Turn off your computer when you leave 
	
4. User Introduced Attacks
	* Hardware intercepts
	  	* Some chips will get intercepted en route, replaced/modified, and sent to their final destination
	* Backdoored chips
		* Some chips will come off the assembly line with backdoors in them already

4. Malicious hardware to turned off compter
        * Throw a new chip on your computer
	* Keylogger in keyboard
	* NSA Playset: <http://www.nsaplayset.org/chuckwagon>
	
4. Electronic Emissions
        * Read this: <https://en.wikipedia.org/wiki/Van_Eck_phreaking>
	
5. Taking you and your computer and forcing you to give up password
	* "Rubber hose cryptography"
		* <https://en.wikipedia.org/wiki/Rubber-hose_cryptanalysis>
		* <https://xkcd.com/538/>
        * Some encryption tools allow the possibility of multiple partitions, so that multiple passwords can be used. Only one password unlocks what you are actually trying to hide, others open different partitions, and there is no way of proving that there are multiple partition/password pairs... this doesn't work very well legally, but might work. A little bit. 
	    * Legal issues surrounding forced password disclosure
              * There is more constitutional law in this field than you ever expected. Further on courses will discuss how all this plays together but:
	      * Basically, US you are good, plead the 5th, self-incrimination. You'll still probably go down, but not for what is on the hard drive.
	      * Europe, you are going to jail
	      * Most other countries, jail
	      * "Not chill" countries, beaten until you give it up, then jail
	      
	* Biometrics
	   * If your device unlocks with anything on your body, they can just take you and open your stuff. 
	   * Fingerprint/retina/voice/face unlocks are not protected by Constitution, they can just make you unlock these things if they have you. 

# Lockpicking
Lockpicking and other security bypass techniques are very popular in the community, for obvious reasons. Many conferences have lockpick competitions and plenty of people carry picks around, because there is nothing worse than getting locked out of things you are allowed access to, but don't have a key.

Read this: <https://www.art-of-lockpicking.com/how-to-pick-a-lock-guide/>. 
At some point we will figure out getting lockpicks to participants so that they can practice. 
	   
[Visit the course page!](https://academy.hoppersroppers.org/mod/page/view.php?id=947)
