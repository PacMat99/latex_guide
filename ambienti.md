---
title: Ambienti e gruppi
layout: home
nav_order: 6
---

# Ambienti e gruppi

## Gruppi

La struttura di un documento non è rispecchiata solo dalla suddivisione in capitoli, paragrafi e così via.  
Un documento può contenere varie parti che rappresentano unità logiche che vanno racchiuse in un *ambiente*.  
Alcuni esempi di unità logiche sono:

* le formule matematiche in corpo --> *math*
* le formule matematiche fuori corpo --> *displaymath*
* le tabelle a doppia entrata --> *tabular*
* citazioni di brani da altre opere --> *quatation*
* *document* stesso è un ambiente (globale)

In LaTeX si possono raggruppare diversi oggetti per scopi specifici nei seguenti modi:

* inserendo l'oggetto tra parentesi graffe { e }
* inserendo l'oggetto tra \begingroup e \endgroup
* inserendo l'oggetto in un ambiente
* inserendo l'oggetto in una scatola (\mbox, \makebox, \fbox, \framebox)

Tutti questi gruppi possono essere annidati l'uno dentro l'altro in modo coerente.  
Ogni dichiarazione eseguita all'interno di un gruppo ha valenza solo all'interno del gruppo stesso.

Vediamo un esempio di gruppo che definisce una porzione di testo che sarà scritto in *maiuscoletto* (tutto maiuscolo lettere scritte in minuscolo leggermente più piccole di quelle scritte in maiuscolo):

```
{\scshape Testo in Maiuscoletto}
```

Tuttavia il gruppo appena mostrato vuole essere solamente un esempio: per scrivere del testo in maiuscoletto è più corretto utilizzare il comando `\textsc{testo}`.

Facciamo un esempio di citazione con corpo leggermente più piccolo di un testo inglese scritto in corsivo utilizzando un gruppo:
\begin{quotation}
    \small\itshape 
    \begin{otherlanguage*}{english}
        Whether I shall turn out to be the hero
        of my own life, or whether that station will be
        held by anybody else, these pages must show.
    \end{otherlanguage*}
\end{quotation}

## Ambienti

Senza dover scrivere ogni volta tutto il blocco di testo per definire, ad esempio, le citazioni, posso creare degli environment che vanno a definire modelli per gruppi di testo che avranno delle caratteristiche ben precise.

```
\newenvironment{citazione}[1]
{\begin{quotation}\begin{otherlanguage*}{#1}\small\itshape}
{\end{otherlanguage*}\end{quotation}}

\newenvironment{incipit}[1]
{\begin{citazione}{#1}\normalfont}
{\end{citazione}}
```
