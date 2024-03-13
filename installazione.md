---
title: Installazione di LaTeX
layout: home
nav_order: 2
---

# Installare LaTeX 

## Quale versione di LaTeX installare

Ti consiglio di installare la version TeX Live in quanto è una delle distribuzioni più popolari. TeX Live include tutto ciò di cui hai bisogno per iniziare a lavorare con LaTeX, incluso il motore di composizione tipografica, i pacchetti per la formattazione dei documenti, e vari programmi ausiliari. Inoltre, parlerò anche di come integrare un editor LaTeX, come TeXworks, che è spesso incluso in TeX Live, per facilitare la scrittura e la compilazione dei documenti LaTeX.

### Installazione su Windows

Scarica dal sito ufficiale di TeX Live [https://tug.org/texlive/windows.html](https://tug.org/texlive/windows.html) l'installer per Windows ed eseguilo.

Durante l'installazione ti verrà chiesto di scegliere quali componenti installare. È consigliabile scegliere l'installazione completa per essere sicuri di avere tutti i pacchetti necessari.  
Aggiungi TeXworks quando viene chiesto a fine installazione per avere un editor di testo semplice e ben integrato con TeX Live.

### Installazione su macOS

MacTeX è una distribuzione TeX specifica per MacOS che include TeX Live e alcuni editor aggiuntivi. Scaricala da [https://tug.org/mactex/](https://tug.org/mactex/) e apri il file .pkg scaricato per avviare l'installazione.

Segui le istruzioni a schermo per completare l'installazione. Anche in questo caso, potrebbe essere utile optare per l'installazione completa.

### Installazione su Linux

Per gli utenti Linux, TeX Live è solitamente disponibile attraverso il gestore di pacchetti della propria distribuzione.

Per distribuzioni Debian, Ubuntu e derivate apri un terminale e digita:

```
sudo apt update
sudo apt install texlive-full
```

Questo installerà la versione completa di TeX Live.

Su Fedora, Red Hat e derivate usa il comando:

```
sudo dnf install texlive-scheme-full
```
