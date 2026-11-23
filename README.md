# Akkord-apper 🎵

To selvstendige HTML-apper for å øve på besifring og akkordtoner. **Kun kode – ingen samtaler/loggfiler ligger i dette repoet.**

## Filer

| Fil | Beskrivelse |
|---|---|
| `akkordtoner.html` | Versjon 1: enkel øving. Se besifringen, skriv inn akkordtonene, hør svaret ditt, grønt kort ved riktig svar. |
| `akkordtama.html` | Versjon 2: gamification/Tamagotchi. Tamagotchien må mates med riktige svar for å ikke sulte ihjel, XP og level, og gjenstander (🎀🕶️🎩🌸🧣👑) som låses opp ved streaks/levels og kan settes på avataren. |

## Slik kjører man

Åpne filen direkte i en nettleser – **ingen server eller internett nødvendig** (fungerer offline):

1. Last ned eller klon repoet
2. Dobbeltklikk på HTML-filen i Finder/Explorer, eller dra den inn i et nettleservindu
3. Første klikk låser opp lyden (nettleserens sikkerhetsregel)

Tips: I Chrome/Edge/Safari/Firefox, sjekk at adressefeltet viser `file:///...` – ikke åpne filen i en innebygd forhåndsvisning som blokkerer `file://`.

## Funksjoner

- Besifring (akkordsymbol) vises stort; eleven skriver inn akkordtonene
- Noter skrives inn via **pianotastatur med navn på tastene** (svarte tast viser doble navn C♯/D♭ osv., `shift`+klikk gir b), tekstfelt (f.eks. `c e g`) eller tastaturet (`c d e f g a b`)
- Notasjon: **B = B-naturlig** (`h` virker også), **Bb skrives `bb`**; kryss `#`, dobbeltkryss `##`/`x`, b `b` etter bokstaven (f.eks. `eb`, `dbb` = dobbelt-b); oktave 3–5
- Notnavnene vises under notelinjen, rett under hver note
- 🔊 Spill av det man har skrevet (blokk eller arpeggio), «Hør fasit», «Spill hele rekken"
- Notene tegnes på en notelinje (SVG); riktig svar blir **grønt**
- Flere akkordrekker i ulike tonearter (C-dur, G-dur, F-dur, A-moll, D-moll, 7-akkorder, blues, **inversjoner/slasj-akkorder**) + tilfeldig rekke
- **Slasj-akkorder** (f.eks. `G/B`, `C/E`): hint sier hvilken basstone som må ligge nederst, og svaret må ha basstonen lavest (spilles også én oktav ned)
- **Piano med to oktaver** (C4–B5 som standard)
- Notene vises på **notelinje i g-nøkkel** (hjelpelinjer under ved lave noter) – med notnavn under hver note
- v2: Tamagotchi med mat-meter, XP/level, streaks, gjenstandssamling – lagres i nettleseren (localStorage), også «mens du er borte»
- v2: **13 gjenstander i to temaer** – 🌈 rainbow unicorn (enhjørning-horn, regnbue-manke, stjernestøv) og 🤘 black metal (corpsepaint, piggkrage, kjede, pentagram) – låses opp ved streaks/level, og du kan **ha på så mange du vil samtidig** (klikk for å ta av/på)
- v2: Notnavnene vises under notelinjen, rett under hver note
- v2: Ved **level 10** blir tamagotchien **👑 LEGENDARY PER OTTAR 👑** (bilde i gullramme, innebygd som base64 i HTML-filen – vises alltid, også uten `assets/`-mappen; `assets/per-ottar.jpg` ligger fortsatt i repoet)

## Teknologi

Vanilla HTML/CSS/JavaScript – ingen byggesteg, ingen eksterne avhengigheter.
Lyd via Web Audio API, noter/SVG rendres i nettleseren.

Laget med Mistral Vibe.
