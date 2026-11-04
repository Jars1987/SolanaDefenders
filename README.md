# Solana Defenders

A space-shooter for the Solana Breakpoint badge, by [Range](https://www.range.org).
Wallet drainers, scam tokens, mixers and exploiters are coming in wave after wave.
Screen them out before they get to the treasury, and look out for the Lazarus boss.

**Post your score on X to compete in the daily ranking. The top score each day wins the LAMP prize.**

## Install it on your badge

The game is installed from the badge app store, straight from this repository.

1. **Find your badge ID.** On the badge, open **Settings → Identity**. It's the
   eight characters shown there, for example `7Qk2M9xA`.
2. **Open the store** at [solanadefcon.com/store](https://solanadefcon.com/store/).
3. **Point it at this repo.** Enter `Jars1987/SolanaDefenders` in the repository box
   and press **Scan**. Select **solana-defenders**.
4. **Send it to your badge.** Enter your badge ID and press **Send**.
5. **Accept it on the badge.** The badge shows the offer. Press **SELECT** to install.
6. Open **Solana Defenders** from the launcher.

No badge with you? You can play in the browser on the
[virtual badge](https://solanadefcon.com/badge/). Copy its badge ID from the panel
beside the screen and follow the same steps.

## How to play

| Button | Action |
|---|---|
| LEFT / RIGHT | Move |
| SELECT or UP | Fire (hold for auto-fire) |
| CANCEL | Pause |

On the virtual badge, use the arrow keys for the D-pad, **Z** or **Enter** for SELECT,
and **X** or **Esc** for CANCEL.

| Threat | Points |
|---|---|
| Exploit (red) | 40 |
| Scam (orange) | 30 |
| Mixer (yellow) | 20 |
| Drainer (pink) | 10 |
| Lazarus boss | ??? |

Some threats take two hits. The game ends when you run out of lives or a threat
reaches the bottom.

## Enter the daily ranking

When the game ends, the **RANGE ALERT** screen shows your score.

1. Press **SELECT** to open the **Share on X** screen.
2. **Scan the QR code** with your phone. X opens with your post already written:

   > I scored 1234 on Solana Defenders at Breakpoint and I'm going for the LAMP prize. Beat it? @range_org

3. **Press LEFT or RIGHT on the badge** to switch to the score card.
4. **Take a photo of the score card** and attach it to the post.
5. **Post it.**

A post counts for the ranking only if:

- it tags **@range_org**,
- it has a photo of the badge's score card, and
- the score in the photo matches the score in the text.

The highest score posted each day wins the LAMP prize.

To retry from the Share screen, press **SELECT**. **CANCEL** goes back to the title
screen, and pressing **CANCEL** there exits the game.

To find out more about Range, press **DOWN** on the RANGE ALERT screen. It shows a QR
code that links to the Range website.

## For developers

The whole game is one file, [`scripts/solana-defenders/main.lua`](scripts/solana-defenders/main.lua),
written against the [Solana OS SDK](https://solanadefcon.com/os/) (Lua 5.4, 320×240).
The store installs only `.lua` files, so the game writes its own `app.ini` the first
time it runs. That is what gives it its name in the launcher.
