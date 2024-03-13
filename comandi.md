---
title: Comandi in LaTeX
layout: home
nav_order: 5
---

# Comandi per la modifica del testo

- **\emph{testo}** --> enfatizza un testo mettendolo in corsivo
- Il carattere ~ indica di lasciare uno spazio in composizione che però non può essere usato per spezzare una riga.
- **\documentclass** --> indica con quale tipo di documento si ha a che fare
- **\linebreak** --> fa andare a capo dalla parola successiva
- Se un comando richiede degli argomenti, questi vanno messi tra {}. Se le graffe sono vuote semplicemente vengono ignorate nello scritto finale.
- **\textit{italic}** --> cambia lo stile del testo e lo mette in corsivo
- **\setlength{\parindent}{1pc}** --> setta una parametro di lunghezza. \parindent è il valore standard del rientro del capoverso
- **\framebox** --> disegna un rettangolo attorno al testo che viene passato come argomento. Può avere diversi argomenti facoltativi: \framebox[3cm][l-r-s]{esempio}

Esempio di comando con argomento: `\textit{italic}`  
`\textit` = *comando*  
`{italic}` = *argomento*

Ci sono tre tipi di comandi per quanto riguarda la forma:

1. un singolo carattere(spazio, ~, ^, _)
2. backslash e un carattere non alfabetico (simboli di controllo)
3. backslash e una successione di caratteri alfabetici (parole di controllo)

I comandi si distinguono in:

- dichiarazioni --> dichiaro qualcosa che vale da qui in poi
- azioni --> prendo qualcosa e su quel qualcosa compio delle azioni

Esempio di dichiarazione: *\small* --> d'ora in poi scrivi tutto più piccolo.
Esempio di azione: *\textit* --> scrivo una parte di testo in corsivo.
