---
title: Struttura
layout: home
nav_order: 2
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

Ogni documento LaTeX avrà *almeno* le seguenti sezioni al suo interno:

1. `% !TEX encoding = UTF-8` --> Utilizzo della codifica UTF-8 per il documento
2.  --> Definizione del tipo di documento che andremo a scrivere
3. `\usepackage[T1]{fontenc}` --> importo la libreria *fontenc* che permette l'utilizzo di accenti e altri segni di punteggiatura
4. `\usepackage[italian]{babel}` --> importa la libreria per il support della lingua italiana
5. `\begin{document}` --> da qui inizia il documento
6. `\title{Titolo documento}` --> il titolo del documento
7. `\author{Nome autore}` --> il nome dell'autore
8. `\date{}` --> la data di scrittura del documento. Se metto le graffe vuote dico che non voglio la data, mentre se non scrivo *\date{}* viene inserita la data di scrittura del documento
9. `\maketitle` --> Genera il titolo del documento. È necessario perché *title* e *author* sono metadati e se non specificato non vengono mostrati.
10. **Testo del documento**
11. `\end{document}` --> qui finisce il documento

## Note varie

1. Le spaziature e l'andare a capo non hanno alcuna influenza sulla scrittura del documento.
2. Andare a capo due volte lasciando una riga vuota equivale a finire un capoverso e iniziarne uno nuovo.
3. Iniziare un nuovo capoverso comporta un rientro all'inizio del testo.
