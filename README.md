# ghost-mayoker
This is a decompiled (and reconstructed) version of [Ghost Mayoker 1.02](https://www.freem.ne.jp/win/game/5568) by the [Nishikigatsuo team](https://kohada.ushimairi.com/)

## how
This game, like the other ones from them, is made with the [Hot Soup Processor](https://en.wikipedia.org/wiki/Hot_Soup_Processor) programming language. All it took was to run a [decompiler](https://github.com/YSRKEN/HSP-Decompiler) on the executable file to retrieve the start.hsp file which contains the code. From there, I just kept debugging to figure out which thing does what (I renamed the variables and resolved exgoto statements into for loops, mostly).

## yeah
This repository contains the 
- `start.hsp` file, extracted from GhostMayoker.exe;
- the spritesheets extracted from `data.dpm`
  
All of Nishikigatsuo team's games have (at least) these files:
1. the game executable
2. [dsoundex.hpi](http://taillove.jp/mia/plugin/arc/dsoundex.txt) (a plugin for HSP which allows sound playback via DirectSound)
3. **data.dpm** (this files contains the spritesheets and other images, and also ***CODE FOR A PREVIOUS VERSION OF THE GAME*** (i almost decompiled 1.00 accidentally because of this))
4. data
   - music
   - se
   - (the reason why they put the music files separately is unclear, i think that they can't pack it with data.dpm?)

# how to run/build this
## Requirements:
- [Hot Soup Processor script editor](https://github.com/onitama/OpenHSP)
- [The game (as downloaded)](https://www.freem.ne.jp/win/game/5568)
- The contents of this repository

## Instructions:
 1. Extract the contents of the game anywhere you want
 2. Put the contents of this repository into the root folder of the game
 3. Load start.hsp into the script editor (hsed3.exe)
 4. HSP > Run

# Notes
I'd like to iterate that **I don't own any of these assets. All credits goes to rakugan65535 (script) and こうもりEQ (graphics)**
