![[Andorin.png]]
# Caratteristiche
## Il centro del commercio
Dopo la Guerra delle Mezze Lame, Andorin ha rappresentato un simbolo di rinascita e crescita nella regione. La sua posizione strategica tra i Campi di Zefiro, l'Oceano Stretto e il Mar Candido ha favorito una rapida ripresa economica. Le rotte commerciali si sono sviluppate, trasformando Andorin in un importante centro di scambi tra diverse regioni. L'ascesa economica ha diversificato l'industria, modernizzato l'agricoltura e consolidato il ruolo politico della nazione nella regione. Andorin è emersa come un esempio di resilienza, trasformando la devastazione post-bellica in una storia di speranza e prosperità.

## Tra sviluppo e tradizione
Le diverse merci di scambio hanno accelerato la crescita delle città in Andorin, portando a una competizione tra i Baroni della Nobiltà. Tuttavia, invece di entrare in conflitto, hanno scelto di collaborare, compensando le mancanze dei rispettivi territori. Alcune zone abitate da popoli tribali come gli Iruxi e i Koboldi hanno generato attriti con le città a causa del desiderio di espansione di entrambi. Queste tensioni rappresentano una sfida per la stabilità, ma ci sono sforzi in corso per mediare e trovare un equilibrio tra le esigenze di crescita urbana e i diritti delle comunità tribali.

## Il richiamo dell'avventura
Nonostante lo sviluppo civile degli ultimi decenni, Andorin mantiene ancora il suo carattere selvaggio, con molte aree inesplorate e rischi sconosciuti. Avventurieri e mercenari sono attivi nell'offrire i loro servizi a nobili e mercanti, sia per recuperare antichi artefatti sia per fornire protezione durante i viaggi attraverso queste terre ancora poco conosciute e piene di insidie. La presenza di queste figure denota una costante ricerca di nuove scoperte e sicurezza in un territorio ancora selvaggio nonostante lo sviluppo civile in corso.

# Fazioni
```dataview
TABLE Leader FROM "Database/Fazioni" WHERE contains(Regioni, this.file.name)
```

## Gilde
In tutta Andorin si è rafforzato nel tempo il sistema delle gilde. Queste associazioni, a cui aderiscono tutti coloro che esercitano una determinata professione, sono state un punto chiave nella crescita delle città. I nuovi mercanti e artigiani ricevevano aiuti e fondi da parte degli esperti del mestiere, che a loro volta accrescono il loro prestigio.

Tra le gilde principali si trovano quella dei mercanti, dei banchieri, degli artigiani (divise per professione), degli avvocati e degli avventurieri.

## Tribù Iruxi
#ARGOMENTA togli lista
La [[Macchia di Scaglie]] occupa una grande parte della regione e al suo interno vivono diverse tribù di Iruxi.
- alcuni hanno contatti, altri isolati
- Ogni tribù ha una caratteristica e gli iruxi si evolvono seguendo queste caratteristiche
- Alcune più violente come i [[Drakkari]]
- Solcabraccia, Scaglie antiche

# Geografia
Andorin occupa la punta meridionale di [[Eloran]], affaccia sui [[Mari|Campi di Zefiro]] a ovest, sul [[Mari|Mar Candido]] ad est ed è separato da [[Zethana]] a sud dall'[[Mari|Oceano Stretto]]. Il clima è mite, con estati secche e inverni piovosi.

La regione è delimitata a nord dai [[Picchi Selvaggi]] e alterna zone pianeggianti e montuose/collinari. Lungo il continente si estendono le [[Alpi Ruggenti]], attorno a cui crescono ricogliose foreste.

#TODO FIUMI

## Località
```dataview
TABLE Tipo FROM "Database/Località" WHERE contains(Regioni, this.file.name)
```

# Governo
#TODO rivedi un attimo i paragrafi
I Baroni sono ricchi mercanti solitamente, specifica come vengono eletti

Ogni città è governata da un [[Nobiltà di Andorin|Barone]], che esercita la sua influenza anche sui borghi limitrofi, attraverso i [[Nobiltà di Andorin|Cavalieri]]. Ad ogni Barone spetta la gestione dei fondi della città, l’approvazione di richieste e progetti delle gilde.

Il ruolo temporaneo di [[Nobiltà di Andorin|Conte]] aumenta il prestigio della città ma impone anche le responsabilità di aiutare gli altri Baroni e prendere parte in interventi diplomatici a nome dell'intera Andorin.

#TODO rivedi nomi e ok mago di corte
Al Barone sono affiancati solitamente le figure del Capitano delle guardie e del Mago di corte. Il primo si occupa della gestione del corpo dei Legionari assegnati alla città (stabiliti in base a numero di abitanti, rischi di incursioni e altri fattori) e la difesa del territorio.

Il mago, invece, è un inviato dell'[[Accademia di Maktabat]] e si occupa di problemi di natura magica. Spesso prende con se alcuni apprendisti in città e se incontra gente talentuosa garantisce per loro l’ingresso all’Accademia.

## Leggi
L'apparato giudiziario di Andorin è composto dai membri della Gilda degli avvocati, che presiedono i processi nelle varie città. I casi passano prima dai prosecutori, che nominano gli avvocati dell'accusa e della difesa e preparano gli appelli.
#TODO rivedi prosecutore

Per ogni processo viene nominata una giuria. Il giudice emette la sentenza dopo aver ascoltato l'accusa, la difesa e la giuria.

# Insediamenti
```dataview
TABLE Tipo, Livello FROM "Database/Insediamenti" WHERE contains(Regione, this.file.name)
```

# Rapporti
#TODO rapporti con altre regioni, tra fazioni, tra insediamenti La chiesa non è ben vista

# Popolazione
Le città sulla costa vantano la maggior diversità di razze di tutto il continente. Nani, Elfi, Umani, Gnomi ma anche creature più rare come Goblin e Iruxi riescono a integrarsi nella vita cittadina. Gli Iruxi selvaggi si concentrano principalmente nella [[Macchia di Scaglie]], anche se alcune tribù occupano le caverne sparse per tutta la [[Costa d'Argento]]. Non è raro vedere gruppi di Iruxi accompagnati da Goblin (generalmente più a nord) o Koboldi, in cerca di alleati.

## Personaggi Importanti
```dataview
TABLE Info, Posizione FROM "Database/Personaggi" WHERE Regione = this.file.name
```

# Religione
Tutte le città presentano una Basilica, un luogo di culto in cui è possibile venerare diverse divinità.

#TODO descrizione dell’architettura

Ogni basilica è gestita da un gruppo di Funzionari, specializzati in diverse religioni.

#TODO rivedi un attimo, religione libera In tutte le città è presente un luogo di culto dedicato alla Primi. Data la diversità delle persone che vivono sul territorio non è difficile trovare anche luoghi in cui vengono praticate altre religioni.

Ogni città ha un Arcivescovo, solitamente un emissario proveniente da Rylorwyn, che si prende cura del luogo di culto.

# Storia
#TODO rivedi qualche nome

## Anno 0 | Post-Frattura
La regione era occupata da diversi gruppi di draghi cromatici. Si autodefinirono draghi nobili, diedero alla loro stirpe il nome di "Covata reale", e battezzarono il loro dominio Andorin, in draconico "Terra dei Re". Diverse tribù di Iruxi, Koboldi e alcuni Goblin che occupavano la regione iniziarono a venerarli come se fossero divinità e offrivano loro beni e ricchezze. Mentre i territori dei Lucertoloidi si espandevano, i draghi divenivano sempre più pirgri e incauti, ormai viziati dalle continue offerte delle tribù.

## Anno 645 | La conquista Imperiale
L'Impero Vastaliano che dominava Rylorwyn, dopo diverse esplorazioni ad Andorin decise di iniziare la conquista. Grazie alla magia runica si fecero strada nel territorio dei draghi e fondarono Emperia sulle coste della Baia Cinta. Oltre che all'espansione, l'Impero era interessato anche ai draghi, da cui ricavavano armi e armature resistenti. Nacquero i Drakenjager, gli Ammazzadraghi, un gruppo di soldati addestrati appositamente per cacciare e distruggere gli allora sovrani di Andorin. Le loro uova divennero i doni per i maghi dell'Accademia e altre potenti figure. I Lucertoloidi non poterono nulla davanti alle armi e agli incantesimi dell'impero e fuggirono per rifugiarsi nelle caverne al di sotto della Costa d'Argento. In pochi decenni quasi tutti i draghi furono uccisi e il regno draconico ebbe fine.

## Anno 704 | La guerra delle Mezze Lame

L'espansione Imperiale nella regione era lenta e i gruppi ribelli ed esiliati iniziarono ad unirsi per fermarla. L'Unione, formata dai ribelli imperiali e le forze di Goramar, Niruta e Ceneria decise di iniziare il contrattacco durante il passaggio delle truppe imperiali in un altopiano del sud di Andorin. I ribelli sotto copertura tra i soldati dell'Impero incisero delle croci sui loro elmi per essere riconosciuti e raggiunto l'altopiano le forze dell'Unione sferrarono un attacco a sorpresa. La Battaglia degli Elmi Segnati fu lo scontro che diede inizio alla guerra delle Mezze Lame, chiamata così per la forma delle armi incise di rune utilizzate dall'Impero e le armi spezzate dell'Unione. Sull'altopiano morirono molti soldati di entrambe le fazioni e da allora quel luogo fu conosciuto come l'Altopiano degli Elmi Infranti. La presa dell'Impero si fece sempre più debole, nuovi gruppi di ribelli continuavano ad insorgere e nuove città iniziarono a sorgere dagli accampamenti militari.

## Anno 716 | La nuova nazione
Terminata la guerra con la sconfitta dell'Impero, la nuova Magocrazia di Kasmona suggerì di usare la zona di Andorin come ponte diretto tra il nord e il sud di Eloran. Si venne a formare una nuova nobiltà, di cui facevano parte anche figure provenienti da Niruta, Goramar e Ceneria. Il compito di questi nobili era di permettere ad Andorin di fiorire come centro commerciale e separarsi dalla nobiltà che aveva caratterizzato l'Impero fino ad allora. Il popolo dei Lucertoloidi si divise. Alcuni di loro chiesero asilo alla nuova nazione, divenendo in pochi anni parte integrante della società mercantile che si stava creando. Altri invece decisero di rimanere fedeli alla loro cultura, abitando le Isole Scagliose a largo della Costa d'Argento. Un altro gruppo però ha reagito in modo violento alla nuova nazione. Questa fazione, nota come i Drakkari, iniziò a causare molti problemi ai Baroni, attaccando i mercanti erranti e occasionalmente i borghi vicini alla costa.

## Anno 721 | Il primo Gran Palio
Il modello di governo suggerito da Kasmona era molto efficace in termini economici e in pochi anni le città riuscirono a fiorire, ma l’assenza di un governo centrale iniziava a pesare sui rapporti tra i Baroni. La competizione si fece sempre più feroce, ogni città voleva trionfare sulle altre, per ricchezze, bellezza, manifatture o qualsiasi altro settore. I baroni allora decisero di sfidarsi in battaglia, per stabilire una volte per tutte chi fosse il migliore. Così ad Ambermoore si tenne il primo Gran Palio, in cui i Baroni mettevano in campo i loro migliori cavalieri, arcieri, maghi e artisti in diverse competizioni. Fu il barone di Ambermoore il primo a vincere, divenendo il primo “Conte del Commercio”, un titolo fittizio, ma riconosciuto dagli altri Baroni. Il suo compito sarebbe stato gestire tutte le questioni riguardanti l’intera nazione di Andorin, in cambio di favori e compensi per la sua città. L’evento fu un grande successo, così tanto che lo stesso Conte decise di ripetere l’evento ogni 4 anni, dando a tutti i baroni l'opportunità di assumere la sua carica.