##  Phishing for Passwords – Chaos-Style Walkthrough (Day 02)

> *"Trust no message that breathes urgency. Verify all senders—even if they speak in the name of reindeer."*

In the grim darkness of Toyville’s inbox, the true enemy is **complacency**. Day 02 teaches us that firewalls won’t save you when an elf clicks a link out of curiosity, panic, or misplaced trust. This is **social engineering**—or as I call it, *soul-fishing with phishing lures*.

But fear not! As a pen-tester (and devout student of digital decay), I’m here to **simulate the heresy so others may repent**.

---

###  Step 1: Deploy the Fake Login Shrine

This is your trap—a convincing imitation of the TBFC portal that **captures credentials** like a Plaguebearer collecting boils.

1. Navigate to the challenge directory:
   ```bash
   cd ~/Rooms/AoC2025/Day02
   ```
2. Launch the phishing server:
   ```bash
   ./server.py
   ```
   → It starts listening on `http://0.0.0.0:8000`  
   → Replace `0.0.0.0` with your **AttackBox’s CONNECTION_IP** when sending the link  
3. **Test it yourself**: Open Firefox on the AttackBox and visit `http://10.82.153.2:8000/`.  
   → Yep, that fake login page? That’s your bait.
   <img width="953" height="642" alt="image" src="https://github.com/user-attachments/assets/e3aa7987-04df-46c4-8044-13d73f0c29c7" />


>  Nurgle’s Wisdom: *“The best traps look like gifts.”*

---

###  Step 2: Cast the Lure with SET (Social-Engineer Toolkit)

Time to send a message so believable, even a cautious elf might click.

1. Start SET:
   ```bash
   setoolkit
   ```
   <img width="871" height="442" alt="image" src="https://github.com/user-attachments/assets/4e96aaf7-7fd5-44c1-833f-679ae9d36371" />

2. Follow the menu:
   - `1` → Social-Engineering Attacks  
   - `5` → Mass Mailer Attack
   <img width="576" height="286" alt="image" src="https://github.com/user-attachments/assets/ead61e03-5402-4976-b3ce-f8913bbe2d2b" />

   - `1` → Single Email Address  

3. Fill in the deception:
   - **To**: `factory@wareville.thm`  
   - **From address**: `updates@flyingdeer.thm` *(impersonate the shipping partner!)*  
   - **From name**: `Flying Deer`  
   - **SMTP server**: `[MACHINE_IP]` *(the target mail server)*  
   - **Port**: `25` *(default SMTP)*  
   - **Subject**: `Shipping Schedule Changes`  
   - **Body** (plaintext):
     ```
     Dear elves,
     Kindly note that there have been significant changes to the shipping schedules due to increased shipping orders.
     Please confirm the new schedule by visiting http://[CONNECTION_IP]:8000
     Best regards,
     Flying Deer
     ```
   - Type `END` (all caps) when finished.
<img width="1057" height="427" alt="image" src="https://github.com/user-attachments/assets/05f690e2-58ea-43ac-b4a6-3b9f09fa8ead" />

>  Khorne’s Note: No attachments. No malware. Just **pure psychological warfare**.

---

###  Step 3: Watch the Terminal for Sacrifices

Return to your `server.py` window and **wait 1–2 minutes**.

If the target clicks and logs in…  
→ **Their credentials appear live in your terminal.**  
→ One elf has fallen. The Gift-Giver’s realm is vulnerable.

This isn’t failure—it’s **proof** that awareness training *must* include **S.T.O.P.**:

- **S**low down  
- **T**ype the URL yourself  
- **O**pen nothing unexpected  
- **P**rove the sender (check the *real* email address!)

---

###  Why This Matters (Beyond the Lulz)

This drill mirrors **real-world threats**:  
- Phishing now lives in SMS (*smishing*), voice calls (*vishing*), QR codes (*quishing*), and DMs.  
- Even cautious users slip when urgency + authority collide.  

As a future **security engineer**, I don’t just break systems—I **reveal human vulnerabilities** so we can build better defenses.  

And maybe… enjoy the irony that **Chaos preaches what security practices already know**:  
> *“The weakest link was never the code. It was the click.”*

<img width="655" height="471" alt="image" src="https://github.com/user-attachments/assets/7198ae9b-f9c1-4a78-8e24-779b08047dd0" />
