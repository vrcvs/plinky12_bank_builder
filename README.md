# Plinky 12 Bank Builder

Unofficial, free, offline webapp to create multisample banks for Plinky 12 from your own samples. Made by [VRCVS](https://www.instagram.com/vrcvs/).

## How to use

1. Open the page and drop up to 8 samples. Name each file with its note: `piano_C3.wav`, `Eb2.wav`, `sax-060.wav`.
2. Set the bank name and artist folder.
3. Choose **Banks loaded together** (1 to 4): how many of your banks you want to play at the same time.
4. Pick the instrument type: **Piano / one-shot** or **Wind / strings / voice (loop)**.
5. Choose an output folder (or download a ZIP) and create the bank.
6. Copy the `artists` folder into `PLINKY/BANKS/` on the card. Back up the card first.

Each bank gets 8 presets (00 to 07). Your samples are processed only in your browser: nothing is uploaded.

## Memory: how many banks at once

Plinky 12 keeps the samples of every loaded sound in 14 MB of memory (about 114 s of audio). The **Banks loaded together** option sets how much audio one bank may use, so that the chosen number of banks fits:

| Banks together | Audio per bank | Size | Per note (8 samples) | For |
|---|---|---|---|---|
| 1 | about 65 s | about 8 MB | about 8 s | one sound at a time |
| 2 | 50 s | about 6 MB | about 6 s | |
| 3 | 33 s | about 4 MB | about 4 s | NEVE (3 voices) |
| 4 | 25 s | about 3 MB | about 3 s | QU4TTRO (4 tracks) |

Long samples are shortened evenly and faded out. Sustained sounds keep looping, so they lose little; pianos and plucks get a shorter tail.

**Sustained sounds (wind / strings / voice)** loop the second half of each note with a crossfade. For a smooth loop the app keeps only the steady part of each note (it drops release tails, gaps and breaths), evens out the level after the attack so the loop does not swell or dip, and does not fade the end of the note to zero. The same bank used on several tracks or voices counts once, and factory sounds are small.

## Credits and license

The tape encoding uses `prepkitchen.js` and related modules from the official Plinky 12 editor by plinkysynth (https://plinky12.com/, https://github.com/plinkysynth/editor), licensed under [CC BY-NC-SA 4.0](https://creativecommons.org/licenses/by-nc-sa/4.0/). This tool is non-commercial and share-alike: derived versions must keep the same license and credit.

## Disclaimer

This tool is unofficial and not supported by plinkysynth. Use it at your own risk. The author is not responsible for any damage to your hardware, memory card or data, or for any loss caused by using it. Back up your card before copying banks to it.

You are responsible for the samples you load. Use only audio you have the right to use.

## Contact

Questions or bugs: Instagram DM [@vrcvs](https://www.instagram.com/vrcvs/) or vrcvsvrcvs@gmail.com.
