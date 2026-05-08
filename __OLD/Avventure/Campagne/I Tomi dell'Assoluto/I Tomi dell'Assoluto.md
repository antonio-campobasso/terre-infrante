-- Immagine
# Diario
## Note
```dataviewjs
const result = await dv.query(`
	LIST
	FROM "Avventure/Campagne/${dv.current().file.name}/Note"
`)

dv.list(result.value.values)
```


## Sessioni
- 2x 13 (libro del tempo, libro della vita )
- 3x 14 (libro delle anime, libro del mare, libro della non-morte)
- 2x 15 (fine viaggio/libro delle ombre, scontro finale)


```dataviewjs
const source = dv.pages(`"Avventure/Campagne/${dv.current().file.name}/Sessioni"`)

for (let group of source.groupBy(p => p.Atto)) {
    dv.header(3, group.key);
    dv.table(["Nome", "Data", "Livello"],
        group.rows
            .sort(k => k.file.link)
            .map(k => [k.file.link, k["Data"], k["Livello"]]))
}

```


# Introduzione
- ambiente, come inizi, perchè inizi, background campagna
- fazioni, guida alla creazione personaggio, house rules
- legami tra personaggi e storia
## Lorem Ipsum
Lorem Ipsum

## Lorem Ipsum
Lorem Ipsum

# Personaggi
```dataviewjs
const result = await dv.query(`
	TABLE Giocatore, Info
	FROM "Avventure/Campagne/${dv.current().file.name}/Comparse"
`)

if(result.value.values.length > 0){
	dv.header(2, "Comparse")
	dv.table(result.value.headers, result.value.values)
}
```

## Giocatori
```dataviewjs
const result = await dv.query(`
	TABLE Giocatore, Info
	FROM "Avventure/Campagne/${dv.current().file.name}/Giocatori"
`)

dv.table(result.value.headers, result.value.values)
```

## NPC 
```dataviewjs
const pages = dv.pages(`"Avventure/Campagne/${dv.current().file.name}/NPC"`)
const source = pages.concat(
	dv.pages(`"Database/Personaggi" and #i-tomi-dell-assoluto`)
)

for (let group of source.groupBy(p => p.Fazione)) {
    dv.header(3, group.key);
    dv.table(["Nome", "Info", "Ruolo", "Posizione"],
        group.rows
            .sort(k => k["Posizione"])
            .map(k => [k.file.link, k["Info"], k["Ruolo"], k["Posizione"]]))
}
```

# Riferimenti
## Fazioni

## Insediamenti
```dataviewjs
const pages = dv.pages(`"Avventure/Campagne/${dv.current().file.name}/Insediamenti"`)
const source = pages.concat(
	dv.pages(`"Database/Insediamenti" and #i-tomi-dell-assoluto`)
)

for (let group of source.groupBy(p => p.Regione)) {
    dv.header(3, group.key);
    dv.table(["Nome", "Tipo", "Livello", "Abitanti"],
        group.rows
            .sort(k => k.file.link)
            .map(k => [k.file.link, k["Tipo"], k["Livello"], k["Abitanti"]]))
}
```

## Luoghi

## Oggetti
