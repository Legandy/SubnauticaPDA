# No Man's Sky - Subnautica PDA Voice Mod
<p align="center"><img src="https://raw.githubusercontent.com/Legandy/SubnauticaPDA/main/.site/icon.png" width="512" height="288">


## Downloads:
[NexusMods][nm]

## Beschreibung:
Dieser Mod ersetzt die Standardstimme des Exosuits durch die Stimme des Subnautica-PDAs. Natürlich aus dem ersten Subnautica.

Ich liebe Subnautica, und No Man’s Sky fühlt sich für mich wie ein Weltraum-Subnautica an.
Einer der Reize von Subnautica war der PDA und die manchmal lustigen und kultigen Sprüche.
Dieser Charme eines KI-Assistenten fehlt in NMS.
Ich wurde nostalgisch, also habe ich diesen Exosuit-Ersatz erstellt.

## So Habe Ich Es Erstellt:
Die meisten Sprachzeilen habe ich aus dem [Leitfaden für benutzerdefinierte Stimmen][cvg] bezogen, den Rest habe ich selbst transkribiert [NMS-Sprachzeilen][nmsVL].
Die Originalzeilen und die Zeilen im Subnautica-Stil findest du in der Tabelle.
Ich bin offen für Verbesserungsvorschläge zu den Zeilen – füge einfach einen Kommentar zur entsprechenden Sprachzeile hinzu und hinterlasse hier einen Kommentar.
Zuerst habe ich versucht, die originale TTS-Stimme „Amy“ und Audacity zu verwenden, war aber mit dem Ergebnis nicht zufrieden, und die Skalierbarkeit hätte mehr Zeit in Anspruch genommen, als ich aufwenden wollte.
Dann fiel mir [Piper TTS][pipertts] ein.
Ich habe auf [Hugging Face][hf] nach einem Sprachmodell gesucht und fand erfreulicherweise ein Sprachmodell für den [Subnautica-PDA][spda].
Ich habe ein [csv2PiperTTS-Skript][2pttsscript] geschrieben, das eine vom Benutzer erstellte „voice_lines.csv“-Datei (exportiert aus einer zweispaltigen Tabelle, Beispiel im [Blatt][sheet-ref]) verwendet und die gesamte Arbeit übernimmt – von der TTS über die Geschwindigkeitssteuerung bis hin zur Lautstärkekorrektur.
Anschließend habe ich die .wav-Dateien mit dem [sound2wem-Skript][2wemscript] in .wem-Dateien konvertiert.
Ich erkläre das alles, weil ihr eure eigene Exosuit-Stimme selbst erstellen könnt.
Du musst nur Glück haben, dass bereits jemand ein Sprachmodell erstellt hat, das dir gefällt, oder du erstellst dein eigenes – dabei kann ich dir allerdings nicht helfen.


## Konflikte:
– Es kann jeweils nur ein benutzerdefiniertes Exosuit-Sprachmodul installiert sein


## Fehler:
– Das Subnautica-PDA-Sprachmodell spricht manchmal undeutlich (vielleicht nicht ausreichend trainiert, ich weiß es nicht)
- Es gibt einige Sprachansagen, die aufgrund eines Fehlers in „No Man’s Sky“ nicht ersetzt werden können
- Die Audiodateien selbst haben einen Pegel von -12 [LUFS][lufs-ref] und sind somit laut genug; ich habe es mit höherer Lautstärke versucht, aber im Spiel ändert sich die Lautstärke nicht.
- Aufgrund einer Einschränkung des Spiels ist die neue Exosuit-Stimme immer leiser als das Original.


## Installation:
- Vortex sollte funktionieren
- Für die manuelle Installation entpacke den Inhalt der Datei „SubnauticaPDA_ExosuitVoice.zip“ in deinen Ordner „No Man's Sky\GAMEDATA\MODS“
- [Weitere Details hier][mg]


## Danke:
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