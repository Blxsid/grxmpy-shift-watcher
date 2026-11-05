**Grxmpy — Shift Watcher**

**Problem**  
Open shifts required a near-immediate response. If I wasn’t already watching my phone, the window closed and the shift was gone. Before Grxmpy, my claim rate was 1 out of 3.

**What it does**  
Grxmpy runs continuously on my iMac (locked screen, always on). It watches incoming shift messages, extracts the claim value, and sends it back immediately so I can claim the shift. Messages mirror to my iPhone, so the system can act even when I’m not at the computer.

**How it works**
- Listens for open-shift messages
- Extracts the claim value
- Checks availability against my Google Calendar
- Sends the claim value through Signal as soon as it’s viable
- Uses Hermes Agent to manage preferences and let me enable or disable the bot remotely via Signal
- Receives a cron summary from Hermes Agent with the result of each run

**Result**  
Claim rate improved from 1/3 to 3/3. The system removes the requirement that I be actively watching my phone when a shift appears.

**Next improvements**
- Stricter calendar conflict rules
- Optional confirmation before claiming higher-value shifts
- Simple logging for claim rate and response timing
