---
Regioni: Andorin
---
![[Legione di Bronzo.jpg]]
# Descrizione
Un gruppo di mercenari caratterizzato dalle decorazioni di bronzo presenti sulle loro armature. Sono assoldati da tutti i [[Nobiltà di Andorin|Baroni di Andorin]] in qualità di guardie delle città. Non rifiutano l’uso della magia, ma preferiscono farne a meno e concentrarsi unicamente sulla tecnica e sul fisico.
## Editti
- Lorem Ipsum
## Anatema
- Lorem Ipsum

# Punti di Interesse
```dataview
TABLE Fazioni, Regioni FROM "Database/Località" OR "Database/Edifici" WHERE contains(Fazioni, this.file.name)
```

# Gerarchia
Il rango di un legionario è mostrato attraverso le decorazioni sulla sua armatura.

- **Generale** (A capo della legione)
	- **Centurione** (Si occupa dell’addestramento di una Centuria, indossa una mantella blu)
	- **Tribuno** (A capo dei legionari di una città, indossa una mantella rossa)
		- **Prefetto** (A capo dei soldati di un borgo o del quartiere di una città, indossa spallacci decorati)
			- **Soldato** (Assegnato ad un prefetto, indossa un elmo decorato)
				- **Recluta** (Appartiene ad una centuria)

Ogni recluta durante l’addestramento può scegliere uno dei seguenti allenamenti:

-   **Oplita** (Combattente in mischia)
-   **Ricognitore** (Combattente leggero/dalla distanza)
-   **Auxilia** (Unità di supporto)

# Membri
L’addestramento da recluta a soldato dura circa un anno, durante il quale la recluta è assegnata ad un gruppo di 100 reclute detto Centuria, sotto il comando di un Centurione. Ogni centuria è composta da 60 opliti, 25 ricognitori e 15 auxilia.

Le centurie sono molto unite e spesso sono viste marciare per tutta Andorin per addestrarsi.

```dataview
TABLE Info, Ruolo, Allineamento, Posizione FROM "Database/Personaggi" WHERE contains(Fazione, this.file.name)
```

# Storia
Originariamente la Legione era un gruppo mercenario assoldato dalla Couronne per combattere nella [[Guerra delle Mezze Lame]]. Si distinsero negli scontri per la loro abilità e al termine del conflitto decisero di restare ad [[Andorin --old]], stabilendo la loro sede nei pressi di [[Brinefort]].

Da allora sono succeduti 3 generali e il secondo, Enea Tullius riuscì a stipulare nell’anno 718 i Patti Aurei con i Baroni delle città. Da allora la Legione sarebbe diventata il corpo di guardia ufficiale di ogni città. Riorganizzò inoltre la Legione per darle una struttura più militare.