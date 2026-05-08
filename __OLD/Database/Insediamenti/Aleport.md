---
Livello: 9
Tipo: Città
Abitanti: 12
Regione: Andorin
---
-- Mappa
# Caratteristiche
#TODO scrivi paragrafo, sistema aspetto

-   Elementi di architettura orientale
-   Città caotica
-   Centro di avventurieri, diversi negozi che provvedono oggetti magici solo per loro

## Abitanti
```dataview
TABLE Allineamento, Info, Ruolo FROM "Database/Personaggi" WHERE contains(Posizione, "Aleport")
```

## Commercio
I grandi spazi pianeggianti fuori dalla città sono dedicati alla coltivazione di grano, malto e luppolo e sono chiamati i Campi d'Oro. Aleport guadagna principalmente dalla lavorazione di questi prodotti, nelle esportazioni di birra e altri derivati alimentari.

```ad-warning
title: Birre rinomate di Aleport
icon: beer
-   **Hozenbrau**: birra rossa dal sapore intenso e alta gradazione. (5cp)
-   **Kandis Kolsh**: birra bionda delicata e bassa gradazione. (3cp)
-   **William Weissber**: birra scura dal sapore fruttato, disponibili in vari gusti. (4cp)
-   **Dylan Debrail**: birra chiara forte. (2cp)
-   **Pinus Pils**: birra bionda scura, non filtrata. (3cp)
- IPA
- BUDS
- LAGER
- STOUT
```

# Edifici
```dataview
TABLE Tipo, Fazioni FROM "Database/Edifici" WHERE contains(Posizione, "Aleport")
```

# Punti di interesse
### Vicia Magis
#TODO: scrivi paragrafo
-   Quartiere in cui dimorano i nobili
-   Spesso si tengono banchetti e feste a cui sono invitati i commercianti più ricchi

#TODO: approfondisci
Le mura che circondano il quartiere appartengono alla prima colonizzazione Imperiale.

# Quest
#TODO rivedi
🥉 La birra di Hozen è acida, qualcuno l'ha contaminata con una strana sostanza venduta da un misterioso mercante che appare solo di notte.

🥈 La gilda degli avventurieri organizza una spedizione nelle caverne infestate dai ragni a nord. Il barone vuole un oggetto all'interno senza farlo sapere ai maghi dell'Accademia.

🥇 Alto livello

# --Note
-   Coltivazioni e allevamenti
-   Centro di commercio, posizione favorevole
    -   Fiume, centro di una regione ecc
-   Governo più complesso
    -   Diversi gradi di nobiltà/amministratori del governo
    -   Guardie più addestrate e numerose
-   Una locanda e un negozio generale
    -   Diversi templi, taverne, artigiani più talentuosi che formano gilde
    -   negozi magici
-   Richieste di aiuto dai borghi associati, organizzazioni criminali e religiose
-   Ricerca di materiali preziosi o attività mercenarie per nobili