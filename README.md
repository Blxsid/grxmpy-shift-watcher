**Grxmpy — Shift Watcher**

**Problem**  
Open shift notifications required a fast response. If you weren’t actively watching your phone, the window closed and the shift was gone. Before Grxmpy, my claim rate was 1/3.

**What it does**  
Grxmpy runs in the background on my iMac (24/7, locked screen). It watches incoming shift messages, extracts the claim value, and sends it back as fast as possible so I can claim the shift. Messages mirror to my iPhone, so the bot can act even when I’m not at the computer.

**How it works**
- Listens for open-shift messages
- Extracts the claim value needed to take the shift
- Checks against my Google Calendar to confirm I’m available
- Sends the claim value immediately through Signal
- Uses Hermes Agent to handle preferences and let me turn the bot on or off via Signal when I’m away from the host
- Hermes Agent sends a cron job with the result of the effort

**Result**  
Claim rate went from 1/3 to 3/3. The bot closes the gap between the shift appearing and me being able to respond, without requiring me to be watching my phone in real time.

**Next improvements**
- Tighter calendar conflict rules
- Confirmation step for higher-value shifts
- Lightweight logging for claim rate and timing
