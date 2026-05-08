---
Regioni: Andorin
---
![[Gilda degli Avventurieri.jpg]]

# Descrizione
La Gilda degli Avventurieri si occupa di raccogliere richiese di aiuto da tutta Andorin, classificarle in base alla difficoltà e stabilire una ricompensa per il completamento. Parte di queste ricompense viene trattenuta dalla gilda. Gli avventurieri possono chiedere di essere assegnati a questi incarichi e formare gruppi per affrontare le sfide più difficili.
Spesso i gruppi di avventurieri sono ingaggiati dai [[Nobiltà di Andorin|Baroni di Andorin]] per partecipare al [[Gran Palio]]

## Editti
- Lorem Ipsum

## Anatema
- Lorem Ipsum

# Punti di Interesse
```dataview
TABLE Fazioni, Regioni FROM "Database/Località" OR "Database/Edifici" WHERE contains(Fazioni, this.file.name)
```

# Gerarchia
Per esprimere il proprio rango, agli avventurieri vengono assegnate due targhette del materiale corrispondente. Su queste vengono scritti il nome e il luogo in cui inviare il proprio corpo in caso di morte.

- **Adamantio** (Capogilda)
	- **Mithral** (In casi molto speciali)
		- **Oro** (Solitamente dal livello 11)
			- **Argento** (Solitamente dal livello 6)
				- **Rame** (Solitamente dal livello 1)
- **Ufficiali di rango** (Di meno man mano che si sale di rango, possono promuovere o cacciare gli avventurieri)

# Membri
Gli avventurieri iscritti alla gilda sono liberi di agire come meglio preferiscono, con la possibilità di avanzare di grado al completamento degli incarichi. Molti mercanti forniscono degli sconti in base al rango dell’avventuriero.

Prima di essere ammessi o di avanzare di rango, gli avventurieri devono superare una prova, in cui si verificano capacità di combattimento, sopravvivenza e lavoro di squadra. Di questo si occupano gli Ufficiali, anche solo suddivisi in ranghi. Il loro compito è anche intervenire nel caso di comportamenti negativi da parte degli avventurieri.

```dataview
TABLE Info, Ruolo, Allineamento, Posizione FROM "Database/Personaggi" WHERE contains(Fazione, this.file.name)
```

## Gruppi della Gilda
### I Camminatori dell'Etere
#### Astrid
Astrid è una guerriera di nobile discendenza, cresciuta nelle ricche terre delle città umane. Ha un'abilità innata con la spada e l'armatura, imparata durante la sua educazione aristocratica. Tuttavia, ha abbandonato la sua vita di agi per cercare avventure e dimostrare il suo valore in combattimento. Astrid è coraggiosa e determinata, ma talvolta si sforza di adattarsi alla vita all'aperto e alle sfide della vita selvaggia.

#### Thorne
Thorne è un mago itinerante noto per la sua curiosità insaziabile e la sua passione per la ricerca di conoscenza arcanica. Porta sempre con sé un libro magico antico e il suo bastone incantato. È l'intellettuale del gruppo, risolvendo enigmi e affrontando minacce magiche con abilità. Tuttavia, la sua sete di conoscenza può talvolta metterlo in situazioni rischiose.

#### Sylas
Sylas è un abile cacciatore di tesori e ladro d'arte, con un occhio acuto per gli oggetti di valore. È furtivo e astuto, esperto nell'aprire serrature e superare trappole. Anche se può sembrare egoista a prima vista, Sylas è legato al gruppo da un senso di cameratismo e si dimostra un amico leale quando è necessario.

#### Eowyn
Eowyn è una cacciatrice esperta con un arco e una freccia, abilissima nel combattimento a distanza e nell'esplorazione dei boschi. È riservata e misteriosa, preferendo la compagnia degli animali e della natura a quella degli esseri umani. La sua saggezza nelle terre selvagge e la sua abilità nel seguire le tracce sono inestimabili per il gruppo.

#### Grom
Grom è un gigante dai capelli rossi, noto per la sua forza sovrumana e il suo temperamento infiammabile. È cresciuto tra le tribù barbariche delle montagne e ha un profondo legame con la natura. Grom è il cuore e la forza bruta del gruppo, spesso lanciandosi in azioni impulsive ma valorose.

# Storia
La gilda è stata fondata da Elora qualche anno dopo la fine della Guerra delle Mezze Lame. All’inizio era formata solo da un gruppo di volontari, che si occupavano di respingere incursioni di Iruxi o creature selvagge nei punti più esterni della città. Dopo che il numero di volontari che seguiva Elora si fece elevato, decise di fondare la gilda, comprando una vecchia locanda e ristrutturandola in quello che oggi è la Lama Ricurva.