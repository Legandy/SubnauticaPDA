# No Man's Sky - Subnautica PDA Voice Mod
<p align="center"><img src="https://raw.githubusercontent.com/Legandy/SubnauticaPDA/main/.site/icon.png" width="512" height="288">


## DOWNLOADS
[NexusMods][nm]

## DESCRIPTION:
This mod replaces the default exosuit voice with the voice of the Subnautica PDA. Of course, of the first Subnautica.

I love Subnautica and No Man's Sky feels like space Subnautica.
One of Subnautica's charm was the PDA and the sometimes funny and iconic lines.
This charm of an AI assistant is not present in NMS.
I felt nostalgic so I made that exosuit replacement.

## HOW I CREATED IT:
I got most of the voice lines from [Custom voices guide][cvg], the rest I transcribed myself [NMS Voice Lines][nmsVL].
You can find the Original and the Subnautica themed lines in the sheet.
I'm open for better changes to the lines, just add a comment to the corresponding voice line and leave a comment here.
First I tried to use the Original TTS Amy Voice and Audacity but wasn't satisfied with the result and the scaleability would have consumed more time than I wanted.
Then I remembered [Piper TTS][pipertts].
I searched for a voice model on [Hugging Face][hf] and I gladly found a voice model for [Subnautica PDA][spda].
I wrote a [csv2PiperTTS script][2pttsscript] that uses a user created voice_lines.csv (exported from a two column spreadsheet, example in the [sheet][sheet-ref]) that does all the job from TTS, speed control and loudness correction.
After that, I converted the .wav files to .wem files with the [sound2wem script][2wemscript].
I'm explaining all that because you can make your custom exosuit voice yourself.
You just need to be lucky that someone already created a voice model you like or create your own, but I can't help you with that.


## CONFLICTS:
- You can only have one custom exosuit voice mod installed at a time


## BUGS:
- The Subnautica PDA voice model slurs sometimes (maybe not enough trained, I don't know)
- There are a few callouts that can not be replaced due to a bug in No Man's Sky
- The sound files itself have -12 [LUFS][lufs-ref] so are loud enough, I tried louder but in game the volume doesn't change. 
- Due to a limitation of the game, the new exosuit voice will always be more quiet than the original.


## INSTALLATION:
- Vortex should work
- For manual installation, extract the contents of the SubnauticaPDA_ExosuitVoice.zip file into your No Man's Sky\GAMEDATA\MODS
- [More details here][mg]


## SPECIAL THANKS:
- [Aquaaa123][a123] for the [Subnautica PDA voice model][spda]
- [RangerDulann][rd] for the [Custom voices guide][cvg]
- [EternalLeo][el] for the [sound2wem script][2wemscript]


[nm]: https://www.nexusmods.com/games/nomanssky/mods/3893/
[mg]: https://docs.google.com/document/d/18k5VfvzLXbpBrAGGO7LK30c2Ta_lWQ5F5YgEpuwKZ6M/edit?tab=t.0#heading=h.vm4bcr5uj28i
[pipertts]: https://github.com/OHF-Voice/piper1-gpl
[hf]: https://huggingface.co/
[spda]: https://huggingface.co/Aquaaa123/piper-tts-pda-subnautica
[2pttsscript]: https://github.com/Legandy/csv2PiperTTS
[sheet-ref]: https://docs.google.com/spreadsheets/d/1iJITjDQPowqthtOQ1yQ2GJlxNoG69EX-0iK6lBr8Wzk/edit?gid=0#gid=0
[cvg]: https://www.nexusmods.com/nomanssky/mods/168?tab=description
[2wemscript]: https://github.com/khossyy/wem2ogg
[lufs-ref]: https://en.wikipedia.org/wiki/LUFS
[a123]: https://huggingface.co/Aquaaa123
[rd]: https://next.nexusmods.com/profile/RangerDulann?gameId=1634
[el]: https://github.com/EternalLeo