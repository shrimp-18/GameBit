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

Session : 2hours
![image](https://github.com/user-attachments/assets/669e1ae0-b301-494e-99e2-2d23064e947f)

25th May, 2025
By this time i realised by sending stuff on #electronics and smart hardware ppl that the usb c thingy wasnt really gonna work.So after more browsing and talking to chatgpt i settled on this chatgpt response. I figured I could just use the cable that the rpi  usually uses, and for portability I could use an <expensive> rechargable battery pack.
I also realised that the kicad symbol for the rpi i had been using all along were WRONG. So i found the correct symbol and footprint from a website and uploaded the files to my kicad preferences and did the assign footprint thingy (again all this took me long to figure out how to do bcs i havent used kicad before and i was learning how to use the software)

Session :2hours
![image](https://github.com/user-attachments/assets/e67396e4-7910-484c-8e57-b7a99b6e5b34)

26th May,2025
After a lot of searching for the footprint and symbol of the lcd screen i had chosen for my game console, i learned that we cant find every footprint and that i could just use a mounting pin instead. So i made connections for my screen from that 1X8 Mounting pin to rpi02w.

Session: 1hour
![image](https://github.com/user-attachments/assets/59b108d0-f9f1-458c-9f7e-7b8f90aab3e9)

11th June,2025
Started figuring out a BOM.

Session: 1hour

13th June,2025
Went crazy searching for the perfect tactile push buttons on jlcpcb and lcsc. The perfect size(settled on 8x8mm using a wonderful reference image i found), the perfect datasheet(bcs everything is in CHINESE rahhh), the right amount of pins etc etc .
![image](https://github.com/user-attachments/assets/b34bce8d-ea65-46f5-ae73-076cfff75b33)
![image](https://github.com/user-attachments/assets/5f2340f5-0a6a-4fe3-a15b-5227cd804da5)

Session: 3 hours

14th June,2025
Connected buttons to rpi 
![image](https://github.com/user-attachments/assets/91ac2898-a283-4980-b12a-b8bdb8a46d08)

Session :30 mins
Made a pdf in canva regarding all the stuff i had completed on gamebit and some stuff which i planned to do which i will attach in my repo.
Session:30 mins
I found this repo which alexren linked on his game console guide: https://github.com/jackw01/pi-tin/ . The schematic is simply beautiful and helped me ALOT in the later stages on making this schematic. ![image](https://github.com/user-attachments/assets/60cb42de-8102-48e5-b2b7-4005d8b8cc8f)



15th June,2025
Researched about audio modules and wanted to find smth better than MAX98357A but i ended up using the same. So added it to my schematic and connected it to rpi.
Session:2 hours
![image](https://github.com/user-attachments/assets/bc28884d-1d2d-4957-b062-30be70c305cc)


I was trying to find the perfect speaker for the next 2-3 days for mannyyy hours on jlc and lcsc. 
![image](https://github.com/user-attachments/assets/5fb2222b-b9c6-4638-a651-17857f333267)

20th June,2025
I had decided on what speaker i was going to use so i added i made its footprint using the datasheet (one hell of a task).
I also made the footprint for the buttons i had chosen earlier. 
Session :2hours

25th June,2025
Searched more buttons to be used for on/off mechanism. I also learned how software+ power on/off worked so i used a tactile button of the software shut doen(bcs we dont wanna fully cut the power) and a slide button for power on/off bcs we wanna completely cut of the power.
Added this to my schematic. After all foorptints were assigned i made my pcb file :yay:
![image](https://github.com/user-attachments/assets/c45e35a5-19a5-4e45-b571-51dceb895d7f)
Also polished all the connections on my rpi and put a lot of GND labels.
![image](https://github.com/user-attachments/assets/9a317258-74aa-43da-a60c-ef66c3682854)
Session: 2hours

26th June,2025
Started working on the pcb which was very easy compared to the schematic. Today i just eyeballed  stuff and arranged everything in a very rough format.
![image](https://github.com/user-attachments/assets/a95fab39-1aa6-40d9-be81-d169f3de3951)
Session:30 mins

27th June,2025
Used correct measurements from datasheets to make the final pcb . Ran DRC.
![image](https://github.com/user-attachments/assets/a91aaa34-f188-428e-bd29-416247c36ed8)

Session:1hour

28th June,2025
Routed connections
Session:30 mins

and just like that the game console GameBit is finally completed. Will focus on making a 3d printed case on fusion360 later. 
ps: the hours are not inflated but im a newbie and researching stuff takes a lot of time 😭
Lmao its somehow came out to Total :24 hours 
