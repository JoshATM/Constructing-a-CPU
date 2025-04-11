# Constructing a CPU

### Key Words:
Accumulator (ACC)
Central Processing Unit (CPU)
Erasable Programmable Read-only Memory (eprom)
Electrically Erasable Programmable Read-Only Memory (eeprom)

#

I have a very limited idea of how to build a cpu apart from being a first year student studying computer architecture.
The aim of the project is that I want this cpu to work, it doesn't have to be fast, it doesn't have to be applicable in real world applications, it just has to work as a cpu.

For this project I am going to use a 16 bit rom and 8 bit ram so then I can call to the ACC 

#

-This comment was made a lot later than when I originally started planning for this project but  I have come to the conclusion that I may have ever so slightly overestimated the time it would take for me to complete this project and even though I'm no electrical engineer, I am still deeply fascinated in how computers work and because I learn best by doing so I will see how long it will take me to create one core of a 16 bit cpu.

#

I have made a square wave generator (the clock) using a 555 timer, hopes and prayers. I have also check the signal using (compared to professional ones) a cheap oscillator.
--- Image ---

#

I have made a 16 bit counter that counts up to 65536 (or 2^16) as my ROM can store 64k x 16 bit instructions.
--- Image ---

#

The first working prototype's code (102b 3000 1040 3001 2100 3002 f000) only officially works with the adder, I have not tested any other method as I am currently in the middle of finding out how to use the ram bidirectionally, instead of the input and output being different.
