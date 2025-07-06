---
Title: GameBit! Game Controller
Author: Neha A.
Description: A cuter and better GameBoy micro
Created_At: 24th June,2025
---
(I didn't journal v actively as I was building this game console, so a lot of it is taken from my friend's DMs whom i regularly updated and my ChatGPT history)

10th May, 2025
The day I first started pondering the idea, I researched existing game consoles like the Hackapet, Sprig, and Pi-tin console etc.
Also saw a hell lot of yt tutorials on how game consoles are made, and also how to use kicad...bcs this is my second hardware project 
first was hackercard on easyeda.
Session: 3 hours (4pm to 7pm)

11th May, 2025
I decided to make something like the Game Boy Micro. Browsed a lot on LCSC, JLCPCB, and Waveshare on what hardware components to use.
For the mcu i settled on rpi 02W. Also found a good 2 inch lcd display on waveshare. Set up my kicad.
Session: 3 hours (8pm-11pm)

15th May,2025
In my schematic i made a system for the rpi to send data and power through a usb c cable which i thought would be useful (in the later stages i eventually remove it)
Also turns out that the connections i made were probably wrong.
![image](https://github.com/user-attachments/assets/669e1ae0-b301-494e-99e2-2d23064e947f)
Session : 2hours

25th May, 2025
By this time i realised by sending stuff on #electronics and smart hardware ppl that the usb c thingy wasnt really gonna work.So after more browsing and talking to chatgpt i settled on this chatgpt response. I figured I could just use the cable that the rpi  usually uses, and for portability I could use an <expensive> rechargable battery pack.
I also realised that the kicad symbol for the rpi i had been using all along were WRONG. So i found the correct symbol and footprint from a website and uploaded the files to my kicad preferences and did the assign footprint thingy (again all this took me long to figure out how to do bcs i havent used kicad before and i was learning how to use the software)
![image](https://github.com/user-attachments/assets/e67396e4-7910-484c-8e57-b7a99b6e5b34)
Session :2hours

