# Constructing a CPU

### Key Words:
Accumulator (ACC)
Central Processing Unit (CPU)
Erasable Programmable Read-only Memory (eprom)
Electrically Erasable Programmable Read-Only Memory (eeprom)

#

Although I have some earlier versions and some later versions, I don't plan on changing anything after 22/04/2025 but you never know what's going to happen. Also Images are from different times as some are through development and some are after.
Images may not be great quality because I took them on my phone, then put them on my pc to then take a screenshot and then to paste into github as they weren't appearing and I suspect it was because they were too big in file size.

#

I have a very limited idea of how to build a cpu apart from being a first year student studying computer architecture.
The aim of the project is that I want this cpu to work, it doesn't have to be fast, it doesn't have to be applicable in real world applications, it just has to work as a cpu.

For this project I am going to use a 16 bit rom and 8 bit ram so then I can call to the ACC 

#

-This comment was made a lot later than when I originally started planning for this project but  I have come to the conclusion that I may have ever so slightly overestimated the time it would take for me to complete this project and even though I'm no electrical engineer, I am still deeply fascinated in how computers work and because I learn best by doing so I will see how long it will take me to create one core of a 16 bit cpu.

#

I have made a square wave generator (the clock) using a 555 timer, hopes and prayers. I have also check the signal using (compared to professional ones) a cheap oscillator.
![image](https://github.com/user-attachments/assets/6c3ffd6f-172b-4d13-9e1b-c2c2a63da535)
![image](https://github.com/user-attachments/assets/66585ab4-cddd-4115-97ea-60004d881e66)

#

I have made a 16 bit counter that counts up to 65536 (or 2^16) as my ROM can store 64k x 16 bit instructions. When I branch I can only access the first 128 (2^8 (cause of my 8 bit ram)) but I don't think I'll be using anywhere near that many instructions* and even if I do then I just need to make sure I don't need to branch to them. *I do want to maybe at some point make a gpu core to render out to a vga output or something similar as it is simple but I haven't started thinking about how I could do that or how I could even implement it into my cpu but I would like to do it eventually.
(I know it's just an image but trust me it works, I'll add a video later when the whole thing works)
![image](https://github.com/user-attachments/assets/49da99e0-0011-4f55-b970-65c4962b3206)

#

The first working prototype's code (102b 3000 1040 3001 2100 3002 f000) only officially works with the adder (2100), I have not tested any other method as I am currently in the middle of finding out how to use the ram bidirectionally, instead of the input and output being different.
