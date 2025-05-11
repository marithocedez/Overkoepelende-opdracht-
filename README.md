# Overkoepelende-opdracht
## Pomodoro timer 

## Binaural beats and breathing light
### Projectbeschrijving
In dit project werd een ontspanningstoestel ontwikkeld dat twee technieken combineert: binaural beats en een breathing light. 
De gebruiker bedient het systeem met in totaal 4 drukknoppen:
- Één om het nummer door te spoelen
- Één om het nummer terug te spoelen
- Één om het nummer te stoppen
- Één om de breathing light te starten of te stoppen

Het doel van dit project is om een eenvoudige, fysieke interface te creëren die gebruikers ondersteunt bij mindfulness, focusmomenten of stressreductie.

FOTO EINDPRODUCT

### Technische uitwerking
De schakeling is opgebouwd uit een Arduino Nano, met een DFPlayer mini voor audioafspeling vanaf een MicroSD-kaart. De audio wordt weergegeven via een luidspreker, en de visuele ademhaling wordt gesimuleerd met een NeoPixel ring. De componenten zijn verbonden via jump wires op twee breadboards.

Gebruikte componenten:
- Arduino Nano
- DFPlayer Mini
- MicroSD-kaart (met 6 mp3-bestanden)
- 4 drukknoppen
- NeoPixel ring
- 1kΩ weerstand (voor spanningsdeling op DFPlayer RX)
- speaker
- breadboards + jump wires

FOTO SCHAKELING

De DFPlayer mini werkt in een loop van zes verschillende geluiden. Zodra het zesde nummer is bereikt begin het systeem opnieuw bij nummer één wanneer er op de "volgende"-knop wordt gedrukt.

Oorspronkelijk was het de bedoeling om de breathing light automatisch te activeren tijdens het afspelen van de muziek. Ondanks de vele pogingingen bleek het technisch moeilijk om deze functies betrouwbaar te combineren met dezelfde knopstructuur. Na meerdere iteraties is ervoor gekozen om de lichtbediening los te koppelen en een aparate vierde knop toe te voegen.
Dit bleek achteraf ook een gebruiksvriendelijke keuze: de gebruiker kan nu zelf bepalen of het licht nodig is, wat het systeem flexibeler maakt.

### Arduino code
De code die voor deze schakeling gebruikt werd is terug te vinden via deze link:
LINK NAAR CODE

### Behuizing
De behuizing werd bewust eenvoudig en functioneel gehouden. De knoppen zijn duidelijk zichtbaar en goed toegankelijk geplaatst. De breathing light werd centraal gepositioneerd voor optimale visuele impact.
Aanvankelijk was het plan om de speaker extern te laten, maar uiteindelijk werd er beslist om deze mee in de behuizing te integreren. Deze beslissing werd genomen op basis van het feit dat geluid goed doorklinkt door materialen zoals karton of PLA. Voor een toekomstigere versie met een stevigere behuizing (bijv. kunststof of metaal) zou integratie van de speaker noodzakelijk zijn.

FOTO NX BESTAND BEHUIZING
