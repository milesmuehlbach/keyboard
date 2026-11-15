---
title: "keyboard"
author: "milesmuehlbach"
description: "A custom 65% keyboard with a rotary encoder."
created_at: "2026-07-09"
---

# #1: GitHub Repo and Planning

- **Date:** July 9, 2026

I spent about an hour setting up the GitHub repo and doing research on different types of keyboards and layouts. I decided on a rotary encoder and a screen, with a 65% layout and tactile switches. I considered an OLED screen but I felt like it was out of scope for my first keyboard project.

![rough layout](imgs/roughlayout.jpeg)
*my rough layout on paper as I tried to figure out what the keyboard would look like*

**Total time spent: 1h 30m**

# #2: Schematic

- **Date:** July 10 2026

I put together the keyboard schematic in KiCad using a Raspberry Pi Pico, 68 key switches, and a diode for each key. I also included a rotary encoder with a push switch. It took me a while to settle on layout design and just get the general feel for kicad, as well as understanding how keyboards work under the hood. I'm following [keeb's](https://keeb.hackclub.com/docs/getting-started/) tutorial for this project.

![schematic](imgs/schematic.png)

**Total time spent: 2h 30m**

# #3: YAY TRACING!!! and layout

- **Date:** July 12 2026

I laid out the keyboard PCB in KiCad, arranging the switch footprints into the keyboard layout and placing the diodes, Pico, and encoder. This ended up taking much much longer than I initially expected because as I went to design I identified many pitfalls in my schematic etc, so I had to go back and modify the layout and schematic multiple times. I then did all the tracing. I had to add room at the top of the board and build a recess for the usb cable bc the traces took up more space than I initially thought. I also added a decent amount of silkscreen with things that are relevant to me! I'm not the best artist so I wasn't able to make it super cool or anything, but svgs of things relevant to me was good enough for now!
![pcb layout](imgs/pcblayout.png)

**Total time spent: 6h**

# #4: Case

- **Date:** Oct 11 2026

Woohoo I finally got the motivation to pick this project back up after like 3 months!!
Time for the case. I've never used onshape before so it took me a little bit to get used to it, but now that I've gotten used to it I now have a basic tray style case. I still need to make the screw holes for the tray and the top plate. Figuring out how they all interface cleanly in cad is just a little bit confusing.
![tray case](imgs/kbdcase1.png)

**Total time spent: 3h**

# #5 Case pt2

- **Date:** Oct 14 2026

I spent a really long time learning more about onshape. I learned about mate connectors and how to fit everything together, and I spent quite a while mateing everything together and then after doing so I realized some of my dimensions were off, so I had to go back and modify quite a few thigns in the case to make sure that everything will work nicely together.
![case w/ pcb](imgs/kbdcase2.png)

**Total time spent: 1h 30m**

# #6 Case pt3 (plate)

- **Date:** Oct 14 2026

I think the plate was the hardest part of building the case; ensuring I was building it in the right place and getting dimensions and spacing right is really hard. I didn't add spaces for my stabilizers because it's hard to model for the stabs if I don't know exactly which model I'm going to use (I haven't put my bom together yet)
![case w/ plate](imgs/kbdcase3.png)

I also modeled the cap for the rotary encoder.
![rotary encoder cap](imgs/rotarycap.png)

**Total time spent: 3h 30m**

# #7 final board yay

- **Date:** Oct 15 2026

I finished!! (for the most part; plate doesn't have stabs because they're not super standard so I'll cad them in when the stabs arrive) 
I added a material to the case and put together a bom, and did the final assembly!
![final board](imgs/finalboard.png)

**Total time spent: 30m**

# #8 fixing things for review

- **Date:** Oct 25 2026

After being rejected once, I added chamfers to my case to improve the aesthetic and also added more 3dmodels to my repo, and improved a few other things.

<img width="304" height="361" alt="image" src="https://github.com/user-attachments/assets/5694a9fa-a41d-42be-ae68-d81ec922d5d3" />

**Total time spent: 5m**

# #9 oh shit i bought the wrong thing

- **Date:** Nov 4 2026
  
so i went to micro center to buy my switches and keycaps. i chose cherry mx brown plus these super awesome keychron keys (coming in a later journal ;))

issue is.. i maybe sorta kinda accidentally bought cherry profile instead of dsa, which means the height of the keycaps isn't uniform across the different rows. it was open box on clearance okay??

anyway i really like these keycaps and want to keep them so I turned it into a happy accident! I modelled a 5 degree incline to my case!

<img width="865" height="414" alt="image" src="https://github.com/user-attachments/assets/cdf25aac-a0da-46a4-905a-bcb057e56d43" />

<img width="728" height="427" alt="image" src="https://github.com/user-attachments/assets/37068d65-d5f3-45f4-a7ae-842401c23ff8" />

**Total time spent: 20m**

# #10 solder header pins to pi pico

the pi pico arrived, so I decided to go ahead and solder the header pins using my pi pico! nothing much else to say, pretty straightforward.

<img width="1536" height="2048" alt="DDFC1BAA-D02E-41AC-B5F8-4FA75D50E083_1_102_o" src="https://github.com/user-attachments/assets/79a034bd-14b9-4f85-bb3f-9d2af8a9bfe2" />
<img width="2048" height="1536" alt="5AFA7367-BCC9-4AC8-A2F7-C10A07CA12C7_1_102_o" src="https://github.com/user-attachments/assets/0089a769-ced2-4a8c-b718-fc0f0371c3ae" />

**Total time spent: 13m**

# #11 pcb arried

my pcb arrived!!! I soldered the diodes, pi pico, and rotary encoder onto the pcb. I still need to recieve the rest of my switches before i can do full assembly but they should be arriving tomorrow!

<img width="1536" height="2048" alt="4D3D7D02-E7A4-4580-B4DC-FF161DE46A90_1_102_o" src="https://github.com/user-attachments/assets/3a77c91d-7f2f-4b5f-bc67-d1e8d7a247fc" />
<img width="1536" height="2048" alt="6C23BD46-046C-42B3-AE3D-C5CE6170A65B_1_102_o" src="https://github.com/user-attachments/assets/a2c9db4c-a5f4-4a02-a52a-59bf1e17fe19" />
<img width="1536" height="2048" alt="DEEDD0DC-6DBF-4530-95C9-DECB1D83EEF0_1_102_o" src="https://github.com/user-attachments/assets/fa74136f-3276-43cb-b332-f7e08172f243" />


**Total time spent: 1h 27m**

# #12 stabs in plate

I added the plate mount stab holes to my plate, and also realized that my plate is larger than my 3dp bed so i had to add a split in the plate (it'll be fineeee?)

<img width="951" height="579" alt="image" src="https://github.com/user-attachments/assets/51ce55ec-a6d2-429e-8195-55e0f0eb6486" />

**Total time spent: 32m**

# #13 tray revision

so i realized that when I added the incline to my tray i added it in the wrong direction and so i had to completely reverse it. I also revised it to be slightly better for support, and I also split the tray into two as my 3dp bed can't fit the full thing 🥲

<img width="884" height="505" alt="image" src="https://github.com/user-attachments/assets/890d5773-8f1f-46e5-993b-ee28aa6090c4" />

**Total time spent: 26m**

# #14 case assembly

the case finished printing so I went through the incredibly painful process of removing the supports, then i attached the two halves together

<img width="768" height="1024" alt="E3BB3B3F-F775-41C0-BBB3-F5E2EA6E3707_1_105_c" src="https://github.com/user-attachments/assets/d7b647fa-dfd6-4273-90e1-853399b95170" />
<img width="1024" height="768" alt="F2C330B2-7B80-4435-996E-81DE8BD86657_1_105_c" src="https://github.com/user-attachments/assets/613ef8a8-59ce-4097-8844-a6e611bdca35" />
<img width="1536" height="2048" alt="7D26F956-706C-4F5C-AB30-D46CA39AB2AC_1_102_o" src="https://github.com/user-attachments/assets/bd8071cb-5e6a-4dd5-9579-e4f2e690c60f" />

**Total time spent: 54m**

# #15 final keyboard assembly!!!!

the last of my switches finally came so I did the full assembly!! I first attached all of the switches to the plate, then soldered each onto the board, then attached all the keycaps and made sure the firmware worked!   
somehow, and I don't know how, everything just worked! except for the stabs; they're super stiff which means that i can't use any keys rn that use the stabs.. which are kind of some of the most important keys so I can't really use the keyboard just yet 💀

<img width="1024" height="768" alt="1404F7F5-916E-4588-AEF5-6D8C4357FE8E_1_105_c" src="https://github.com/user-attachments/assets/4635345d-7cc4-4472-ab06-8dd744077668" />
<img width="2048" height="1536" alt="B4464644-BDF8-4B5B-B0A5-4022189416B5_1_102_o" src="https://github.com/user-attachments/assets/2dd028de-3180-4082-ade9-cbdf76f71189" />

the stabs had these little notches that I didn't cad into the plate so I had to cut out of the plate with pliers lol
<img width="768" height="1024" alt="A23FC60E-1DD2-44DF-A335-D7F561D46438_1_105_c" src="https://github.com/user-attachments/assets/de9c133c-c623-4a65-a13b-dbe2bf0025da" />

**Total time spent: 2h 13m**

