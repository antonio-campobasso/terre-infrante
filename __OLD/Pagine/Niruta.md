-- Immagine
# Caratteristiche
NIruta è una regione prevalentemente desertica, con poche città sparse lungo oasi e rive dei fiumi che tagliano il grande deserto di Bahrlimar. Tutte le città sono sotto il controllo del Sultano Al-Malik, ma molte di esse operano con una certa autonomia, considerando la limitata attenzione che il Sultano riserva al suo popolo.

In epoche remote, questa terra era abitata dal potente popolo dei Dokimiani, di cui restano oggi soltanto tracce negli antichi edifici e artefatti risalenti a oltre 1000 anni fa, disseminati nel deserto. La loro scomparsa dopo la Frattura ha aperto le porte ai nomadi Mashawa, un popolo errante che ha plasmato la regione secondo le proprie tradizioni.

Il commercio qui si basa principalmente su spezie rare che prosperano nel clima arido, sulle stoffe pregiate ottenute dal Lino delle Sabbie, una pianta unica che cresce sulle rive dei fiumi, e sulle materie prime ricavate dalle carcasse dei mostri erranti nel deserto. La Gilda dei Cacciatori Sayidi organizza audaci spedizioni per cacciare queste bestie colossali e rivendere le parti.

Il commercio degli artefatti antichi recuperati nelle antiche rovine Dokimani è altrettanto rischioso, considerando che il deserto cambia forma ad ogni tempesta di sabbia, disorientando anche gli esploratori più esperti.

In aggiunta, tribù nomadi di orchi, provenienti dalle formazioni rocciose di Mal’Zagh, si sono recentemente spinte più vicino alle città, minacciandole con saccheggi e incursioni.



- Ya'qub Quamar Ad-Din Dibizah
- Khalid Kashmiri
- Khidir Karawita
- Ismail Ahmad Kanabawi
- Usman Abdul Jalil Sisha
- Muhammad Sumbul

## Lorem Ipsum
Lorem Ipsum



# Fazioni
Lorem Ipsum

```dataview
TABLE FROM "Database/Fazioni" WHERE contains(Regioni, this.file.name)
```

## Lorem Ipsum
Lorem Ipsum

# Geografia
Lorem Ipsum

## Località
```dataview
TABLE Tipo FROM "Database/Località" WHERE contains(Regioni, this.file.name)
```

## Lorem Ipsum
Lorem Ipsum

# Governo
Lorem Ipsum

## Leggi
Lorem Ipsum

# Insediamenti
```dataview
TABLE Tipo, Allineamento, Livello FROM "Database/Insediamenti" WHERE contains(Regione, this.file.name)
```

# Rapporti
Lorem Ipsum

# Popolazione
Lorem Ipsum

## Personaggi Importanti
```dataview
TABLE Info, Allineamento, Posizione FROM "Database/Personaggi" WHERE Regione = this.file.name
```

# Religione
Lorem Ipsum

# Storia
Lorem Ipsum