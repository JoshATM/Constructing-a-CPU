# Constructing a CPU

### Key Words:
Accumulator (ACC)
Central Processing Unit (CPU)
Erasable Programmable Read-only Memory (eprom)
Electrically Erasable Programmable Read-Only Memory (eeprom)

### Parts:
UV Eraser:
https://www.aliexpress.com/item/1005006494154448.html?spm=a2g0o.productlist.main.3.51275dcfpmBotF&algo_pvid=7a36646c-baac-4806-9811-78d8dd3ef73b&algo_exp_id=7a36646c-baac-4806-9811-78d8dd3ef73b-1&pdp_npi=4%40dis%21GBP%219.15%218.69%21%21%2182.32%2178.20%21%40211b819117335969497133804e9a5b%2112000037408905026%21sea%21UK%213423784242%21X&curPageLogUid=LmbrF2uceAYu&utparam-url=scene%3Asearch%7Cquery_from%3A
Adjustable DC Power Supply:
https://cpc.farnell.com/tenma/72-2685/power-supply-0-30v-3a-1ch/dp/IN07633?st=tenma%20dc%20power%20supply
Eprom:
https://www.aliexpress.com/item/4000830498536.html?spm=a2g0o.order_list.order_list_main.5.4dc41802JlwAm7
Wall adapter for the UV Eraser:
https://www.aliexpress.com/item/1005005678174399.html?spm=a2g0o.order_list.order_list_main.11.4dc41802JlwAm7
Crocidile clips for the dc power supply (so it would be easier when working with the breadboard):
https://www.aliexpress.com/item/1005007407275225.html?spm=a2g0o.order_list.order_list_main.17.4dc41802JlwAm7
4-bit D-register:
https://www.aliexpress.com/item/1005003680716317.html?spm=a2g0o.order_list.order_list_main.23.4dc41802JlwAm7
Full Adder:
https://www.aliexpress.com/item/1005005948018959.html?spm=a2g0o.order_list.order_list_main.29.4dc41802JlwAm7
Pack of electronics (it was just better value for money) such as NAND, NOR, NOT, AND, OR Gates, Hex Inverting Schmitt Trigger (which we are not using), a 3-to-8 Line Decoder, and some Shift Registers:
https://www.aliexpress.com/item/1005007101157170.html?spm=a2g0o.order_list.order_list_main.35.4dc41802JlwAm7
XOR Gates:
https://www.aliexpress.com/item/1005004780916462.html?spm=a2g0o.order_list.order_list_main.41.4dc41802JlwAm7
Multiplexer:
https://www.aliexpress.com/item/1005001869847746.html?spm=a2g0o.order_list.order_list_main.47.4dc41802JlwAm7
Wires:
https://www.aliexpress.com/item/1005006914127180.html?spm=a2g0o.order_list.order_list_main.53.4dc41802JlwAm7
Comparators:
https://www.aliexpress.com/item/1005007505549635.html?spm=a2g0o.order_list.order_list_main.59.4dc41802JlwAm7
555 IC:
https://www.aliexpress.com/item/1005002606088465.html?spm=a2g0o.order_list.order_list_main.23.6e451802MEbdn0
RAM:
https://www.aliexpress.com/item/1005006807832121.html?spm=a2g0o.order_list.order_list_main.77.6e451802MEbdn0



## Parts
The UV eraser is so I am able to clear the memory of the rom as it is an eprom and not an eeprom or flash memory. If you did want to use an eeprom then it could be a lot cheaper as the eeprom is erased by using electric signals instead of UV rays and you don't need an adjustable dc power supply to get (in this case) 12.75 volts to write to the eprom.
The Adjustable DC power suplly that I have can support up to 30v but the highest for my specific rom is 13V and the cheapest one I can find (that's decent) is below which can support uo to 18V.
https://cpc.farnell.com/duratool/d03233/power-supply-1ch-18v-3a-adjustable/dp/IN08000?st=dc%20adjustable 



Also sidenote, if you happen to have a GQ-4X4 or a TL866II Plus laying around, then it will be a lot easier then using a raspberry pi (arduino uno may be better but I only had an arduino nano so I didn't want to start multiplexing bits) but I've already spent enough money, I didn't want to spend anymore for something that I may only use once to read and write 16 bit roms.


I have a very limited idea of how to build a cpu apart from being a first year student studying computer architecture.
The aim of the project is that I want this cpu to work, it doesn't have to be fast, it doesn't have to be applicable in real world applications, it just has to work as a cpu.

For this project I am going to use a 16 bit rom and 8 bit ram so then I can call to the ACC 
