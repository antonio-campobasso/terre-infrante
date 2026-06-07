---
Regioni:
  - Andorin
Personaggi Importanti: "[[Martin (Sindorak)]]"
---
![[Covata Reale.jpg]]

# Descrizione
Un tempo il gruppo di draghi cromatici più numeroso nelle Terre Infrante, occupava tutta la regione di [[Andorin --old]] e comandava decine di tribù di [[Iruxi]] e [[Koboldo|Koboldi]]. Dopo lo sterminio da parte dell’[[Impero di Västil]] i pochi membri rimasti si nascondono lontano dagli insediamente oppure al loro interno in forma umanoide.

## Editti
- Lorem Ipsum

## Anatema
- Lorem Ipsum

# Punti di Interesse
```dataview
TABLE Fazioni, Regioni FROM "Database/Località" OR "Database/Edifici" WHERE contains(Fazioni, this.file.name)
```

# Gerarchia
- Dopo la conquista imperiale rimane solamente la figura del Sovrano e della Levatrice Reale

- **Sovrano** (Solitamente il più anziano dei draghi, la sua volontà è assoluta)
	- **Vassallo** (Governa un territorio seguendo gli ordini del sovrano)
		- **Levatrice** (Protegge e accudisce le uova dei vari vassalli)
	- **Levatrice Reale** (Protegge e accudisce le uova del sovrano)

# Membri
Ogni drago è in grado di assumere una forma umanoide.

```dataview
TABLE Info, Ruolo, Posizione FROM "Database/Personaggi" WHERE contains(Fazione, this.file.name)
```

# Storia
Dopo la [[Frattura]] uno stormo di circa 20 draghi cromatici si allontananò dai resti di [[Continenti Antichi --old|Draconia]] e approdarono sulla punta meridionale di [[Eloran --old]] e in poco tempo sterminarono i pochi insediamenti presenti nella regione, lasciando in vita solo tribù di [[Iruxi]] e [[Koboldo|Koboldi]] che accettavano di venerarli.
Furono loro a dare il nome alla regione di [[Andorin --old]], in draconico "Terra dei Re" e si proclamarono "eredi reali" delle più antiche stirpi draconiche.
Nella loro società solo i draghi maschi potevano ambire alle posizioni di Vassallo o Sovrano, mentre le femmine erano limitate al ruolo di Levatrice.
Con il tempo i draghi si indeboliscono, rinunciando a cacciare e facendo affidamento solo alle offerte dei loro sudditi. 
Quando l'[[Impero di Västil]] diede inizio alla conquista di Andorin, i draghi caddero uno dopo l'altro, soprattutto alla divisione dei Drakenjagere.
#TODO storia di agrixia
