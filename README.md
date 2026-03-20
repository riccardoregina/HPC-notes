# HPC Notes

Questo è il repository degli appunti del corso di **High Performance Computing**, tenuto dalla Prof.ssa V. Mele presso l'Università degli Studi Federico II di Napoli nell'Anno Accademico 2025/2026.

**Questi appunti sono destinati a supportare gli studenti nel loro percorso di apprendimento e a fornire una risorsa di riferimento per gli argomenti discussi durante il corso, ma non sostituiscono in alcun modo il materiale ufficiale e le lezioni dei docenti.**

Questo documento è prodotto da studenti, per studenti, e potrebbe contenere errori o imprecisioni. Feedback e correzioni sono ben accetti e incentivati, e possono essere inviati tramite pull request o issue in questa repository.

Il template usato per gli appunti è stato sviluppato da [Riccardo Elena](https://github.com/RiccardoElena). Il repository del template è disponibile [qui](https://github.com/RiccardoElena/UniNotes_Template).

## Compilazione degli appunti

Per compilare il codice sorgente degli appunti, è necessario disporre di un ambiente LaTeX locale come, ad esempio, texlive. Qualora non si abbia già a disposizione un'installazione locale di LaTeX, è consigliato l'uso dell'immagine Docker di texlive. Un esempio di configurazione pronta per l'uso, a patto di avere Docker installato, è presente presso [questo repository](https://github.com/riccardoregina/tex-docker).

### Compilazione

Una volta clonato il repository e configurato l'ambiente LaTeX, è possibile effettuare la compilazione completa degli appunti con:

```bash
pdflatex main.tex
bibtex main
pdflatex main.tex
pdflatex main.tex
```

oppure con: 

```bash
latexmk -pdf main.tex
```

Se non è necessaria una compilazione completa (per compilazione completa si intende la compilazione multipla necessaria al corretto funzionamento di riferimenti e bibliografia), è possibile eseguire:
```bash
pdflatex main.tex
```
Ciò può essere utile per velocizzare la compilazione a seguito di piccole modifiche.

## Struttura della Repository

```bash
HPC-notes/
├── main.tex           # File principale
├── csnotes.cls        # Classe custom degli appunti
├── _files/            # Risorse grafiche
│   ├── _images/          # Immagini utilizzate nel documento
│   └── ...               # Altre file di risorse
└── _chapters/         # Capitoli del documento
    ├── 0_intro.tex
    ├── 1_introduction.tex
    └── ...
```

## Come contribuire

Contributi, correzioni e miglioramenti sono benvenuti. Per contribuire, creare un fork di questo repository ed aprire una Pull Request. Per segnalare errori o problemi, aprire una issue dettagliando il problema riscontrato.

## Autori

- [Riccardo Regina](https://github.com/riccardoregina)

---

**Nota Bene**: Gli appunti sono in continuo aggiornamento durante lo svolgimento del corso.