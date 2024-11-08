# Capture The Flag HacKSU Lesson
### Hosted By Austin Sternberg

## What is a CTF?
CTFs or Capture the Flag challenges are much like the classic game you might have played as a child. CTFs involve two main things:
- There is some kind of flag that obscured from plain view (hidden)
- Some kind of cybersecurity principle hiding the flag

A common and very popular way to find these challenges is to participate in a CTF competition. My personal favorite is Carnegie Mellon's yearly picoCTF event, which is typically held in March or April. These events are typically set up online, though I have seen a few that were in person, typically as part of a hackathon.

### CTF's also tend to break challenges into categories:
- Web Exploitation
- Cryptography
- Reverse Engineering
- Forensics
- General Skills
- Binary Exploitation

Tonight's lesson will go over an easy challenge from each of these categories

The premise of these challenges then is to use a variety of cybersecurity skills and tools to attempt to get the code, file, or website to spit out a flag.

## What are the tools?
Though each CTF is technically different, I can suggest these main tools:

- [dcode.fr](https://www.dcode.fr/)
- [CTF Toolkit](https://ctftoolkit.com/)
- [cyberchef](https://gchq.github.io/CyberChef/)
- [ChatGPT](https://chatgpt.com/)

This is one of the only times were chatgpt is not only allowed, but at times the best tool for the job. That being said, if the other tools can handle it, use them first.

Each of these will provide nearly all of the tools required for any CTF challenge, baring very specific ones. dcode.fr is better for cipher brute-forcing, were CTF Toolkit provides everything else. Cyberchef is not my go-to for cryptographic challenges, but its magic setting is useful when dcode fails.

## How Do I Get Started?
- Make an account on [picoCTF](https://play.picoctf.org/register)
- Click on 'Practice' to enter the challenge gym

## What will this lesson cover?
I am aiming to cover one easy challenge across each of the categories that the pico gym provides. Many of the challenges have been used a actual challenges used in previous picoCTF competitions.

I will be going over the following challenges:
- heap 0
- Mod 26
- CanYouSee
- what's a netcat?
- Transformation
- Scavenger Hunt

My writeups (instructions) for solving these challenges are available as part of this repository. Unlike most write ups, I do not provide the whole flag at the end, as a way to encourage actually trying to follow my steps.

## Additional Resources and Challenges
I want to note here a couple different events/places you can dive deeper into ctfs and similar hacking challenges:

As mentioned, Carnegie Mellon will be hosting their annual PicoCTF sometime in March or April. In the meantime, the Pico Gym has more than 250 challenges you can attempt now.

One of my friends runs a CTF at the Rochester Institute of Technology ([link](https://ctftime.org/ctf/170))

Similar to the gym but more challenging, there is always [TryHackMe](https://tryhackme.com/) and [HackTheBox](https://www.hackthebox.com/). These provide both trainings and cyberrange vms to attempt to find and exploit vulnerabilities in.