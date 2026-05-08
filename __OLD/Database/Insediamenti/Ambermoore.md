---
Livello: 10
Tipo: Città
Abitanti: 16
Regione: Andorin
---
--Mappa
#TODO mappa e scrivi
# Caratteristiche
- 


## Abitanti

```dataview
TABLE Allineamento, Info, Ruolo FROM "Database/Personaggi" WHERE contains(Posizione, this.file.name)
```

## Commercio
- Da sempre rinomata per i prodotti ittici, soprattutto molluschi e murici da cui si ricavano tinture
- I mercanti più ricchi vorrebbero ridurre le zone di pesca per rendere la città un punto commerciale sul Mare Stretto

# Edifici

```dataview
TABLE Tipo, Fazioni FROM "Database/Edifici" WHERE contains(Posizione, this.file.name)
```

# Punti di interesse
## Città Vecchia
#TODO approfondisci
Lorem Ipsum

# Quest

```ad-success
title: Basso livello
icon: butterfly
```

```ad-question
title: Medio livello
icon: wolf-head
```

# Note
- Coltivazioni e allevamenti
- Centro di commercio, posizione favorevole
    - Fiume, centro di una regione ecc
- Governo centrale
    - Cerchia di nobili più importanti degli ordini governativi
    - Guardie più addestrate e numerose
- Una locanda e un negozio generale
    - Attività di ogni tipo
    - negozi magici
- Richieste di aiuto dai borghi associati, organizzazioni criminali e religiose
- Ricerca di materiali preziosi o attività mercenarie per nobili