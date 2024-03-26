---
title: Il primo documento
layout: home
nav_order: 7
---

# Il primo documento in LaTeX

Creare il tuo primo documento in LaTeX è un eccellente modo per iniziare a familiarizzare con questo potente sistema di composizione tipografica. Ecco una guida passo dopo passo per scrivere, compilare e visualizzare un semplice documento LaTeX.

1. Apri il tuo Editor LaTeX
Apri TeXworks o qualsiasi altro editor LaTeX che hai scelto durante l'installazione di LaTeX. Questi editor sono specificamente progettati per facilitare la scrittura di documenti LaTeX fornendo evidenziazione della sintassi, completamento automatico dei comandi e altre funzionalità utili.

2. Scrivi il Tuo Primo Documento
Inizia con un documento semplice per familiarizzare con la struttura di base di un documento LaTeX. Copia e incolla il seguente codice nel tuo editor:

```
\documentclass[a4paper, 12pt]{article}
\usepackage[T1]{fontenc}
\usepackage[english,italian]{babel}

\usepackage{kantlipsum}

\newenvironment{citazione}[1]
{\begin{quotation}\begin{otherlanguage*}{#1}\small\itshape}
{\end{otherlanguage*}\end{quotation}}

\newenvironment{incipit}[1]
{\begin{citazione}{#1}\normalfont}
{\end{citazione}}

\begin{document}

\title{Il mio primo documento LaTeX}
\author{Mattia}
\date{\today}
\maketitle

Questo è il mio primo documento in \LaTeX{}.
Questo è un \textit{capoverso}, il primo capoverso di questo documento.
Se tutto va per il verso giusto le righe successive alla prima dovrebbero essere spostate leggermente più a sinistra perché non hanno il rientro iniziale.

\emph{Vediamo un po' cosa riusciamo a fare!}
Effettivamente tutto sembra funzionare.
Il rientro iniziale ha origini centinaia di anni fa ed è uno stile tipografico a cui non si è ancora trovata un'alternativa altrettanto valida.

\small Questo \`{e} un paragrafo con ``caratteri speciali''.

Ora proviamo a scrivere alcuni esempi di framebox:

\framebox[10cm][l]{framebox con testo a sinistra}

\framebox[10cm][r]{framebox con testo a destra}

\framebox[10cm][s]{framebox con testo distribuito}

{\scshape Questo è un Esempio di Gruppo in Maiuscoletto.}

\textsc{Questo è un Testo in Maiuscoletto scritto in modo Corretto.}

Facciamo un esempio di citazione con corpo leggermente più piccolo di un testo inglese scritto in corsivo utilizzando un gruppo:
\begin{quotation}
    \small\itshape 
    \begin{otherlanguage*}{english}
        Whether I shall turn out to be the hero
        of my own life, or whether that station will be
        held by anybody else, these pages must show.
    \end{otherlanguage*}
\end{quotation}
\`{E} un perfetto esempio dello stile di Dickens.

Ora vediamo un altro esempio.

\kant[1][1-4]

\begin{incipit}{english}
    \kant[2][1-4]
\end{incipit}

\kant[3][1-4]

\begin{citazione}{english}
    \kant[4][1-2]
\end{citazione}

\end{document}
```

Questo codice di esempio crea un documento contenente un titolo, un'autore, una data, e due sezioni: "Introduzione" e "Conclusione".

1. Compila il Documento
Per trasformare il tuo codice sorgente LaTeX in un documento PDF, devi compilare il documento. La maggior parte degli editor LaTeX ha un pulsante o un menu dedicato per fare ciò. In TeXworks, per esempio, dovresti vedere un pulsante verde con una freccia verso destra nella parte superiore della finestra. Assicurati che l'opzione "pdfLaTeX" sia selezionata nel menu a tendina accanto a questo pulsante, poi clicca il pulsante per compilare il documento.

1. Visualizza il Documento
Dopo la compilazione, l'editor dovrebbe aprire automaticamente il documento PDF risultante. Se ciò non avviene, cerca un file PDF con lo stesso nome del tuo documento LaTeX nella stessa cartella dove hai salvato il documento LaTeX. Puoi aprire questo file con qualsiasi lettore PDF per vedere il risultato del tuo lavoro.

1. Modifica e Sperimenta
LaTeX è molto potente e flessibile. Dopo aver creato il tuo primo documento semplice, inizia a sperimentare con altri elementi. Puoi aggiungere elenchi puntati o numerati, inserire immagini, creare tabelle, scrivere equazioni matematiche e molto altro. Ecco un esempio di come inserire un elenco puntato:

```
\begin{itemize}
    \item Questo è il primo punto dell'elenco.
    \item Questo è il secondo punto dell'elenco.
\end{itemize}
```

E per un'equazione matematica:

```
\begin{equation}
    e^{i\pi} + 1 = 0
\end{equation}
```

Inserisci questi blocchi nel corpo del documento e ricompila per vedere i cambiamenti.

Conclusioni
Creare il tuo primo documento in LaTeX può sembrare complicato all'inizio, ma una volta che hai imparato i comandi di base e hai compreso il flusso di lavoro, scoprirai che LaTeX è uno strumento incredibilmente potente e versatile per la creazione di documenti di aspetto professionale. Non esitare a cercare ulteriori risorse e guide online per esplorare le molteplici funzionalità di LaTeX!

Per compilare un documento lanciare il comando `pdflatex nome.tex` da terminale.  
Esempio:

```
pdflatex test1.tex
```
