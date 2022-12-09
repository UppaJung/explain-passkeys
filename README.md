# Explaining *passkeys*

I created this repository because existing explanations of passkeys, from the [FIDO Alliance and the Chromium team](./previous-explanations.md), describe what passkeys are not (passwords), and list the security attributes of passkeys, but never reveal what a passkey actually is. I get that the folks involved with the FIDO have an affiniity for not revealing things, but we should make an exception when asked "what is a passkey?"

So let's fix that!

## What is a passkey?

Passkeys are *login secrets*, like passwords and PINs, but with an extra safety feature: you can create an account with a passkey, and log into that account with that passkey, without ever sending the secret (the passkey) itself. Since the websites you have accounts with never get to see your passkey, your passkey stays safe even if the website is compromised. These safer account setup and login processes are all managed by your browser and use advanced math called *cryptography*.

Aside from the use of cryptography to protect passkeys, these secrets are not much different from the random passwords a password manager can generate for you. Passkeys are 4-5 times longer than most random passwords. You may never notice, or even see a passkey written down, since you should never need to type a passkey or remember it. Your browser stores Passkeys in your password manager. Even you don't have a password manager, Chrome has a Google's password managers built in and Apple's Safari browser has Apple's KeyChain built in. While your browser uses passkeys differently than passwords when you create accounts or login to them, the same rules that apply to storing passwords in a password manager also apply to storing passkeys: (1) if you lose access to the information stored by your password manager, you’ll lose both your passwords and passkeys; (2) if an attacker compromises your password manager, they can steal both your passwords and passkeys.

