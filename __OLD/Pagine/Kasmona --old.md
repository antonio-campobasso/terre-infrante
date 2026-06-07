---
tags:
  - "#i-tomi-dell-assoluto"
  - "#regione"
---
-- Immagine
# Caratteristiche
## L'isola magica
Lorem Ipsum

## Crocevia di culture
stanno anche un gruppo di draghi

# Fazioni
- Principalmente l'accademia
- Ordine di bibliotecari che precede la costruzione dell'accademia
- Draghi sapienti

```dataview
TABLE FROM "Database/Fazioni" WHERE contains(Regioni, this.file.name)
```

## Lorem Ipsum
- Vecchie istutuzioni studentesche diventate riconosciute ufficialmente (alchimisti?)

# Geografia
Lorem Ipsum

- da segnare bosco sussurrante, baia dei draghi, fiume diba

## Località
```dataview
TABLE Tipo FROM "Database/Località" WHERE contains(Regioni, this.file.name)
```

## Lorem Ipsum
Lorem Ipsum

# Governo
- Forte democrazia, non esiste nobilità
- Città indipendenti, del Consolato, di cui fanno parte
	- Sindaco
	- Consiglio Civico
	- Capo degli Araldi
	- Magistrato (a capo dei maghi della città)
- Città piccole possono avere un Assessore che solitamente fa parte del consiglio civico delle grandi città

- I Sindaci e il Rettore sono a stretto contatto

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