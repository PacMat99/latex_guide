---
title: Struttura di un documento
layout: home
nav_order: 3
---

# Struttura di un documento LaTeX

1. Codifica del documento  
   `% !TEX encoding = UTF-8`
2. Formato e classe del documento (article, report, book, suftesi, amsart, amsbook, ...)  
   - `\documentclass[a4paper, 12pt]{book}`
   - *a4paper* per il formato a4
   - *letterpaper* per il formato 'letter' americano
   - *twoside* cambia leggermente la disposizione del testo rispetto ai margini e prepara il documento per la stampa fronte retro
   - *12pt* per definire la grandezza del testo
   - *twocolumn* per scrivere l'articolo in doppia colonna
3. La gabbia è la zone del foglio dove viene composto il corpo del testo
4. La pagina è formata da
   - testatina
   - gabbia
   - piè di pagina
   - Il corpo è una misura della grandezza dei caratteri
5. Il formato ISO A4 è 21cm x 29.7cm (formato derivante dalla radice quadrata di 2 approssimata in millimetri)
6. Preambolo --> nel preambolo vengono specificati i pacchetti aggiuntivi che verranno usati per comporre il documento

Ogni documento LaTeX avrà *almeno* le seguenti sezioni al suo interno:

1. `% !TEX encoding = UTF-8` --> Utilizzo della codifica UTF-8 per il documento
2.  --> Definizione del tipo di documento che andremo a scrivere *(non più necessario in quanto standard)*
3. `\usepackage[T1]{fontenc}` --> importo la libreria *fontenc* che permette l'utilizzo di accenti e altri segni di punteggiatura
4. `\usepackage[italian]{babel}` --> importa la libreria per il support della lingua italiana (1)
5. `\begin{document}` --> da qui inizia il documento
6. `\title{Titolo documento}` --> il titolo del documento
7. `\author{Nome autore}` --> il nome dell'autore
8. `\date{}` --> la data di scrittura del documento. Se metto le graffe vuote dico che non voglio la data, mentre se non scrivo *\date{}* viene inserita la data di scrittura del documento
9. `\maketitle` --> Genera il titolo del documento. È necessario perché *title* e *author* sono metadati e se non specificato non vengono mostrati.
10. **Testo del documento**
11. `\end{document}` --> qui finisce il documento

(1) Si possono usare diverse lingue nel documento scrivendo, ad esempio, `\usepackage[english,italian]{babel}` per indicare che il documento in questione avrà come lingua principale l'italiano e come lingua secondaria l'inglese. *L'ultima lingua specificata è la lingua base.*

## Pacchetti aggiuntivi

In un documento LaTeX possono essere utilizzati pacchetti aggiuntivi che permettono l'utilizzo di funzionalità aggiuntive. In particolare un pacchetto può:

1. aggiungere funzioni non presenti in LaTeX standard
2. modificare la definizione di alcuni comandi standard
3. modificare il valore di alcuni parametri, come per esempio quelli di impaginazione

Se hai bisogno di template aggiuntivi o altro materiale TeX, lo puoi trovare nell'archivio TeX ufficiale [ctan](https://ctan.org/ctan)

## Note varie

1. Le spaziature e l'andare a capo non hanno alcuna influenza sulla scrittura del documento.
2. Andare a capo due volte lasciando una riga vuota equivale a finire un capoverso e iniziarne uno nuovo.
3. Iniziare un nuovo capoverso comporta un rientro all'inizio del testo.
4. Se l'unica lingua usata è l'inglese americano, non è necessario caricare *babel*
5. \usepackage{graphicx} permette l'inserimento di documenti grafici esterni
6. \usepackage{amsmath} permette di scrivere formule matematiche complesse
7. \usepackage{amssymb} permette di utilizzare un gran numero di simboli matematici
8. Se voglio utilizzare diversi pacchetti che non richiedono opzioni posso metterli tutte nello stesso `\usepackage{...}` separati da virgola
