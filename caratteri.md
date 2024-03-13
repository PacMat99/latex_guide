---
title: Caratteri speciali
layout: home
nav_order: 4
---

# Caratteri in LaTeX

Un documento LaTeX può essere scritto utilizzando solo caratteri ASCII compresi nell'intervallo 32-126.  
Ci sono poi i caratteri speciali e quelli specifici per lingua che possono essere scritti utilizzando delle combinazioni di caratteri.

## Caratteri speciali

| Carattere | Nome          | Descrizione |
| :---      | :---          | :---        |
|           | Spazio        | Più spazi equivalgono a un solo spazio. Gli spazi all'inizio di una riga sono ignorati. |
| \         | backslash     | Introduce i comandi. |
| '         | apostrofo     | Funge da apostrofo e da virgoletta alta chiusa. Due apostrofi producono le doppie virgolette alte chiuse. Il comando \\' produce un accento acuto. |
| `         | accento grave | Funge da virgoletta alta aperta. Due accenti gravi producono le doppie virgolette alte aperte. Il comando \\' produce un accento grave. |
| {         | aperta graffa | Insieme a } delimita gli argomenti dei comandi. Per scrivere { devo scrivere \\{. |
| }         | chiusa graffa | Insieme a { delimita gli argomenti dei comandi. Per scrivere } devo scrivere \\}. |
| "         | Doppio apice  | Non si deve usare se non nel comando \\" che produce una dieresi (es. fl\\"{u}gel = flügel). |
| $         | Dollaro       | Serve per cominciare e finire le formule matematiche. Per scrivere $ devo scrivere \\$. |
| ^         | circonflesso  | Si usa nelle formule matematiche per indicare esponenti. Il comando \\^ produce un accento circonflesso (es. H\\^{o}pital = Hôpital). |
| _         | underscore    | Si usa nelle formule matematiche per indicare i pedici. Il comando \\_ produce un underscore. |
| ~         | tilde         | Se usata da sola indica uno spazio in cui non è ammesso spezzare una riga, per esempio per non separare le iniziali dal nome. Il comando \\~ produce una tilde come accento (es. Espa\\~{n}a = España). |
| #         | Cancelletto   | Si usa nelle definizioni dei comandi. Il comando \\# produce un cancelletto. |
| &         | e commerciale | Si usa negli ambienti di allineamento. Il comando \\& produce una e commerciale. |
| %         | percento  | Introduce un commento che non appare nella pagina. Il comando \\% produce un commento. |
