# Andre Økt
## Innføring i Javascript og DOM-manipulasjon

### Hvordan komme i gang:
- `git clone https://github.com/koseprogg/AndreOkt.git`
- Åpne mappen i valgfri teksteditor, for eksempel Visual Studio Code
- Vi skriver spill-logikken i filen index.js
- Gjennom linjen `<script src="index.js"></script>` vil nettsiden vår implementere javascript-logikken vår

## Vi skal lage logikken i følgende funksjoner: 

De 7 vinnerscenarioene i Tic Tac Toe: `[0, 1, 2], [3, 4, 5],[6, 7, 8], [0, 3, 6], [1, 4, 7], [2, 5, 8], [0, 4, 8], [2, 4, 6]`

- `handleCellPlayed(cellClicked, cellClickedIndex)`
  - Skal håndtere å endre tilstanden til cellen som har blitt trykket på.
- `handlePlayerChange()`
  - Skal håndtere å bytte hvilken spiller sin tur det er.
- `handleResultValidation()`
  - Skal sjekke om noen har fått tre på rad, eller om det har blitt uavgjort.
- `handleCellClick(clickedCellEvent)`
  - Skal håndtere at en spiller trykker på en spillrute.
- `handleRestartGame()`
  - Setter spillbrettet tilbake til starttilstanden.


## Nyttige funksjoner for DOM-manipulasjon:
- `document.querySelectorAll(selector)`: Returnerer en statisk liste som representerer DOM-elementene som matcher selector-argumentet
  - Eksempler på selectors: `p`, `.navn-på-klasse`, `#navn-på-id`, `h1`, 
- `document.querySelector(selector)`: Returnerer det første elementet i DOMen som matcher selector-argumentet. Returnerer `null` hvis et element ikke blir funnet.
-  `HTMLElementObject.innerHTML`: Returnerer verdien til `HTMLElementObject`. Lar deg også sette verdien.
- `HTMLElementObject.addEventListener(event, callBack)`: Legger til en eventListener som lytter etter `event`-argumentet, og utfører `callBack`-funksjonen når eventet "fyres av".
  - DOM events: https://www.w3schools.com/js/js_htmldom_events.asp



Ressurser: 
- https://developer.mozilla.org/en-US/docs/Web/API/Document_Object_Model


Neste steg: 
- https://codeheir.com/2019/02/04/how-to-code-pong-1972-1/