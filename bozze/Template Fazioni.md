---
tags: [bozza, template, fazioni]
type: bozza
status: draft
---

# Bozza — Template per le Fazioni

Confronto tra lo stile vecchio (`__OLD/Database/Fazioni/Covata Reale.md`, `Drakkari.md`, `Gilda degli Avventurieri.md`) e quello attuale (`database/Fazioni/Repubblica degli Emir.md`, `Marina Reale.md`, `Corsari.md`, `Penjaga.md`), per capire cosa tenere.

## Cosa cambia tra vecchio e nuovo
- Frontmatter: vecchio usava `Regioni:` (plurale) + a volte `Leader:`/`Personaggi Importanti:`; nuovo usa `base: "[[Fazioni.base]]"` + `Regione:` (singolare, lista) — niente più campo leader in frontmatter, il capo si racconta dentro Membri/Gerarchia.
- Vecchio aveva query dataview su `"Database/Località"` per i Punti di Interesse e su `"Database/Personaggi"` per i Membri — path ormai morti (dataview è stato sostituito dal plugin Bases nativo di Obsidian, gli stessi `.base` già usati per i rimandi Regione nelle pagine nazione).
- Immagine in testa (`![[Nome.jpg]]`, come nel vecchio stile): reintrodotta, più immagini opzionali per Aspetto e Simboli.
- Editti/Anatema sostituiti da **Competenze**/**Obiettivi**: più generici, non presuppongono che la fazione abbia un vero e proprio credo/codice — vanno bene anche per una gilda commerciale o una repubblica mercantile.
- Gerarchia nidificata del vecchio stile resta utile — portata dentro.
- "Gruppi della Gilda" (sottogruppi nominati con membri propri) è un'idea buona del vecchio Gilda degli Avventurieri, utile per fazioni con cellule interne (es. gruppi di pirati, compagnie di corsari).

## Template proposto

```markdown
---
base: "[[Fazioni.base]]"
Regione:
  - [Nome Regione]
---

![[Nome immagine.jpg]]

# Descrizione
[Cosa fa la fazione, che ruolo ha nella regione, che tensioni la attraversano — prosa o elenco puntato, quello che si adatta meglio.]

## Competenze
[In cosa eccelle la fazione: mestiere, risorsa, potere militare/economico/magico distintivo.]

## Obiettivi
[Cosa vuole ottenere, a breve e lungo termine — cosa la muove.]

## Simboli
![[Nome immagine simbolo.jpg]] *(opzionale)*
[Stemmi, bandiere, sigilli, motti — cosa li rappresenta e dove si vedono.]

# Membri
![[Personaggi.base#Nome Fazione]]
[Vista Bases nativa, filtrata sui personaggi con `Fazione` contenente questa fazione, colonne Nome + Ruolo — sostituisce l'elenco manuale. "slot" per posti vacanti restano comunque utili come nota a parte, non essendo personaggi veri.]

## Aspetto
![[Nome immagine aspetto.jpg]] *(opzionale)*
[Come si riconoscono i membri: uniformi, tratti comuni, marchi.]

## Gerarchia
[Elenco nidificato dei ranghi dal più alto al più basso, con una breve descrizione tra parentesi per ciascuno.]

## Sottogruppi
[Solo se la fazione ha cellule/compagnie/ciurme distinte al suo interno, ciascuna con nome e membri propri — vedi "Gruppi della Gilda". Rimuovere la sezione se non serve.]

# Punti di Interesse
![[Luoghi.base#Nome Fazione]]
![[Insediamenti.base#Nome Fazione]]
[Due viste Bases native, filtrate su `Fazione` contenente questa fazione — una per i luoghi, una per gli insediamenti (Bases lavora su una cartella/base per volta, niente combinazione unica come il vecchio `FROM "Località" OR "Edifici"`). Omettere l'embed che resterebbe vuoto.]

# Storia
[Narrazione dalla fondazione a oggi, in ordine cronologico. Usare sottotitoli `### Anno X-Y: ...` se la storia è lunga, come nelle pagine nazione.]
```

## Estensione richiesta ai `.base` (una tantum + per ogni nuova fazione)

Per far funzionare gli embed sopra, serve lo stesso meccanismo già usato per `Regione` nelle pagine nazione, esteso con una proprietà `Fazione`:

1. **Schema (una tantum)** — aggiungere la proprietà `Fazione` (e `Ruolo` per i personaggi) al blocco `properties:` di `Personaggi.base`, `Luoghi.base`, `Insediamenti.base`.
2. **Dati** — aggiungere `Fazione:` (lista) al frontmatter dei personaggi/luoghi/insediamenti coinvolti; ai personaggi aggiungere anche `Ruolo:`.
3. **Per ogni fazione nuova** — aggiungere una view `table` filtrata `Fazione.contains("Nome Fazione")` in ciascuno dei tre `.base` (stesso pattern delle view `Couronne`/`Hale'kai`/`Fjellanag` già presenti), poi embeddarla nella pagina della fazione.

Il passo 3 è manuale e ripetuto per ogni fazione — non evitabile con le Bases attuali (niente self-reference tipo `dv.current()` di Dataview), ma è lo stesso costo già accettato per le viste Regione.

## Domande aperte
1. ~~Editti/Anatema obbligatori o no~~ — risolto: sostituiti da Competenze/Obiettivi, generici per qualsiasi fazione.
2. ~~Immagine in testa~~ — risolto: reintrodotta, più opzionali per Aspetto e Simboli.
3. ~~Punti di Interesse a wikilink manuali~~ — risolto: viste Bases native (vedi sopra). Da confermare solo il nome della proprietà (`Fazione`, coerente con `Regione` già in uso) e se serve retroattivamente sui luoghi/personaggi già esistenti o solo da qui in avanti.

Tutte le domande principali chiuse — resta solo il dettaglio tecnico del punto 3 (retroattivo o no) da decidere quando si comincia a popolare i `.base`.
