# Sounds from the basement: Extreme low-level game cheating

In this talk, we will explore an advanced method for cheating in multiplayer 
PC-based games by leveraging System Management Mode (SMM) as the cheat’s 
runtime environment. SMM, a privileged execution mode in x86_64 processor 
architecture, operates at the lowest level of the CPU privilege rings; 
beneath even the kernel's ring 0 or hypervisor’s “ring -1” - SMM executes in 
so-called “ring -2”. This makes it an ideal environment for executing 
anything undetected by traditional detection software typically running in 
higher privilege rings, be it anti-cheat or anti-virus software.

We will cover the technical details of how to use SMM, its inherent 
advantages over other cheating techniques, and the challenges in interfacing 
with game memory and game object types while remaining undetected from the 
most established anti-cheat platforms. This talk will include a demonstration 
of a working game cheat which can bypass modern anti-cheat tools and a deep 
dive into the potential implications for anti-cheat developers (and other 
security professionals whose job it is to detect malicious activity in their 
context). Attendees will leave with a solid understanding of why SMM is a 
powerful tool for stealth in executing code maliciously and what 
countermeasures might be required to combat such sophisticated attacks.
