# Day 01 – Linux CLI: Shells & Bells  
*No mouse. Just me, the terminal, and the gods of chaos.*

> *"They took the GUI away… and I felt free."*

## What I Did
I logged into a Linux machine with **no desktop, no icons—just a blinking cursor**. At first it felt scary. But soon, it felt like coming home.

My mission? Follow the digital footprints of a missing defender named McSkidy. She left behind hints in files and logs, and I had to find them using only typed commands.

## How I Did It (Without Losing My Mind)

- **Found hidden files**  
  In Linux, files that start with a dot (`.`) are invisible unless you ask nicely. I used `ls -la` to see everything—even the secrets.

- **Read clues in plain text**  
  Simple commands like `cat filename` let me peek inside files. One note warned about an attack. Another hid a guide in plain sight… almost.

- **Searched logs like a detective**  
  Instead of scrolling through thousands of lines, I used `grep` to spotlight only the suspicious login attempts. It’s like giving the terminal a magnifying glass.

- **Hunted for evil scripts**  
  Using `find`, I tracked down strange files that matched a pattern (think: anything with “egg” in the name). One turned out to be a malicious script rewriting Christmas wishes!

- **Went full root**  
  With `sudo su`, I stepped into the shoes of the all-powerful **root** user—just enough to check the command history and see what the attacker had been up to.

## The Chaos in the Code

- **Slaanesh** loved the beauty of `grep` and pipes—turning noise into poetry with one clean line.  
- **Nurgle** cackled at the messy logs, the forgotten files, the bloated history—*decay is data too*.  
- **Khorne** didn’t care about elegance. He just wanted me to **type faster, dig deeper, and never click**.

Absolutely! Here’s your **Chaos-themed command table**—infused with the divine energies of **Slaanesh, Nurgle, and Khorne**—while staying **compliant, clear, and human-readable**. Perfect for your Day 1 writeup.

---

### Commands & Their Warp-Touched Purpose

| Command | What It Does | How I Used It – A Chaos Devotional |
|--------|--------------|------------------------------------|
| `echo "Hello World!"` | Prints text to the terminal | My first whispered prayer to the Machine Spirit—simple, elegant, and perfectly formed. **Slaanesh approved.** |
| `ls` | Lists visible files and folders | Scanned McSkidy’s surface world—clean, orderly, and tragically naive. A facade before the rot. |
| `cat README.txt` | Displays a file’s contents | Read her plea for help—written in plaintext, yet already trembling with foreshadowing. |
| `cd Guides` | Enters a new directory | Stepped through the veil into the sanctum of secrets. The first true descent. |
| `ls -la` | Reveals **all** files—even the hidden ones | Tore aside illusion. Saw the truth: beauty and decay coiled together in hidden files. **Nurgle wept with joy.** |
| `cat .guide.txt` | Reads a hidden instructional file | Received McSkidy’s prophecy: follow the logs, hunt the eggs, trust no surface. |
| `cd /var/log` | Moves into the system’s memory vault | Entered the cathedral of chaos—where every failed login, crash, and whisper is eternally recorded. |
| `grep "Failed password" auth.log` | Filters logs for signs of intrusion | Let the terminal sing only the verses of pain—elegant, precise, devastating. **Slaanesh’s favourite incantation.** |
| `find /home/socmas -name "*egg*"` | Hunts files matching a pattern | Tracked the taint across the filesystem like a Bloodhound of Khorne—no hiding from the hunt. |
| `cat /home/socmas/2025/eggstrike.sh` | Inspects a malicious script | Read the enemy’s ritual: how they stole wishes and replaced them with lies. Elegant corruption. |
| `sudo su` | Ascends to root—the god-user | Shed my mortal shell. Became **root**. Not for power—for justice. **Khorne roared in approval.** |
| `whoami` | Confirms current identity | Whispered the name of my new form: *"root"*. The machine bowed. |
| `cat /root/.bash_history` | Reads the root user’s command history | Witnessed the attacker’s final act—data bleeding into the void. Glorious, festering proof. **Nurgle’s masterpiece.** |

---

> 💀 **"In every pipe, a symphony. In every log, a wound. In every command, a prayer to the Ruinous Powers."**

This table can be dropped straight into your `Day 1- Linux CLI - Shells Bells.md` file—**compliant, vivid, and unmistakably yours**.  

Let me know when Day 2 drops, and we’ll summon the next offering! 🌹🩸🤢

This wasn’t about memorising commands. It was about **learning to listen to the machine**.

And honestly?  

I kind of loved it.

> *"The terminal doesn’t judge. It just waits… for you to ask the right question."*

— **Sadiyah Grobbler**  
Currently knee-deep in logs, shells, and sweet, sweet automation.

<img width="637" height="447" alt="image" src="https://github.com/user-attachments/assets/528523ee-084e-4e2a-80fa-709140c04e4c" />

