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
- Noter skrives inn via noteknapper, tekstfelt (f.eks. `c e g`) eller tastaturet (`c d e f g a h`)
- Norsk notasjon: **H = B-naturlig, B = Bb**; fortegn med `#`/`b` (f.eks. `f#`); oktave 3–5
- 🔊 Spill av det man har skrevet (blokk eller arpeggio), «Hør fasit», «Spill hele rekken"
- Notene tegnes på en notelinje (SVG); riktig svar blir **grønt**
- Flere akkordrekker i ulike tonearter (C-dur, G-dur, F-dur, A-moll, D-moll, 7-akkorder, blues) + tilfeldig rekke
- v2: Tamagotchi med mat-meter, XP/level, streaks, gjenstandssamling – lagres i nettleseren (localStorage), også «mens du er borte»

## Teknologi

Vanilla HTML/CSS/JavaScript – ingen byggesteg, ingen eksterne avhengigheter.
Lyd via Web Audio API, noter/SVG rendres i nettleseren.

Laget med Mistral Vibe.
