# Data Minimization
If your primary risk comes from people you know maliciously or non-maliciously looking through your devices, here are some simple defaults that minimize what you leave as your digital detritus. 

# Incognito Mode:

Does this prevent someone who is monitoring your internet connection, whether a network admin or your Internet Service Provider (ISP) from seeing what websites you are visiting? No.

Does this prevent a forensics expert from determining which sites you've visited? No, but it makes it harder.

Does this keep you from being tracked by advertisers? No, but it can help.

Does this minimize your chances of being embarrassed by your search history and someone looking at your browsing history? Yes. 

There are use cases for Incognito mode but know its limitations.  

# Messages 

## Disappearing Messages 

Disappearing messages can allow you to have a safe default, where you can set the expiration of messages at a point in time in the future. This minimizes the total amount you could leak if your phone/email/chat account was compromised. 

Disappearing messages certainly aren't going to stop someone from saving a message if they want to, but they will make them less likely to be found and saved later, and that can fit your risk model.

## Encrypted Messages

Just because a message is disappearing (cough Snapchat) or encrypted (Telegram's Default), that does not mean it is End to End (E2E) encrypted. E2E guarantees that messages can only be read by the intended recipients, so not even the server owners can read the contents. I personally recommend the Signal app for most needs. 

Signal takes this idea of E2E even farther and does not send Metadata to the servers. This means that even if they wanted to, they are not able to tell which of their users is talking to who, or when. This idea of minimizing metadata is huge. 

As mentioned earlier, if the product is free, the product is you, but in this case... not true! Signal is run by an absolute stud of a cyberpunk named Moxie Marlinspike, and he is the coolest hacker on earth. [Read up on him a bit](https://moxie.org/) and be inspired.

# Full Disc Encryption (FDE)

To go one step further, if your phone or computer is stolen and the contents aren't encrypted, even without the password it is fairly straightforward to just pull all the information from it. With full disc encryption, all data is encrypted at rest and has to be decrypted every time the device boots with a secret key. This means that if someone steals your device and tries to take the data off it they will not be able to, ensuring the confidentiality of your personal files. 

iPhones take this one step farther and encrypt the phone every time the lock screen is set, by default. This secure default has gone a long way towards making Apple the privacy and security company.

If you are on Android, it is possible to enable FDE, but going to lock screen does not encrypt all contents, only shutting down the phone.

For Windows, here is a decent guide: [Microsoft Secure Boot and Encryption Overview](https://docs.microsoft.com/en-us/windows-hardware/drivers/bringup/secure-boot-and-device-encryption-overview). 

If you want to enable this, Google should point you in good directions.

# Encrypted Partitions / VMs

If you are not worried about a technical threat, it is not a terrible idea to work from a VM and just turn it off every time you finish using it. There are a ton of ways that could go wrong, and you could always be instructed by whoever has control of you and the computer to turn it on and unlock it.

Remember, if you are targeted and get hacked on the host computer, you get hacked in the VM as well. Keep that in mind.

So what's the actually secure way to do things on a computer? The generally accepted answer is to mount an encrypted partition in your OS, and use that to hold a VM to do your important work on. If you are interested in this, [here's a guide](https://www.ivpn.net/privacy-guides/creating-a-vm-within-a-hidden-truecrypt-partition/).

That gives you some deniability, especially with the ability to make multiple partitions that unlock to different passwords, but it's not going to hold up particularly well in court, or to someone with a wrench.

# Tails and Other Risk Focused Operating Systems

On the absolute farthest end of the spectrum are security-focused operating systems, which prioritize your data's safety over anything else, especially usability. 

[Tails](https://tails.boum.org/) which runs off of a USB stick and when shutdown erases all the new data created, leaving no trace it was ever run. Think of it like a forensically secure incognito mode for your computer.

If you still want to save files between reboots, there are other options, most notably [Qubes-OS](https://www.qubes-os.org/intro/), that are specifically designed for secure computing. 

If you do all your work in Tails and you only use E2E encrypted messaging that disappears, you are probably pretty safe, and also pretty paranoid. But if your threat model actually requires Qubes or Tails, you shouldn't be getting advice from this website. 

To wrap up, minimize logs, minimize messages, minimize metadata. By applying these defaults you can minimize risk, even without requiring encryption or passwords, which are easily subverted in person.


