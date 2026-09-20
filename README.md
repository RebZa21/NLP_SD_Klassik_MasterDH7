# NLP_SD_Klassik_MasterDH7
Esercitazione NLP MasterDH7 2026-2027 UniMI

# NLP su Sturm und Drang e Classicismo di Weimar

## Scopo del progetto

Lo scopo del progetto è verificare se un classificatore, guardando **solo il lessico** di brevi porzioni di testo (finestre di 200 token), riesce a distinguere i drammi tedeschi dello *Sturm und Drang* da quelli della *Klassik* di Weimar.

- **Corpus:** sei drammi di Goethe, Schiller e Lenz (tre SD, tre Klassik), etichettati secondo la periodizzazione di de Boor/Newald. Goethe e Schiller compaiono in entrambe le classi, quindi il modello non può limitarsi a riconoscere l'autore.
- **Metodo:** TF-IDF e word2vec con regressione logistica, validati con leave-one-work-out (a turno ogni opera è tenuta fuori dall'addestramento).

## Struttura del progetto

```
nlp-sturm-und-drang-klassik/
├── notebooks/
│   └── NLP_SuD_Klassik.ipynb        # Notebook con gli output salvati
├── corpus/
│   ├── die-raeuber.epub
│   ├── friedrich-schiller-wallenstein.epub
│   ├── goetz-von-berlichingen.epub
│   ├── iphigenie-auf-tauris.epub
│   ├── jmr-lenz-der-hofmeister.epub
│   └── maria-stuart.epub
└── docs/
    └── relazione_NLP_SuD_Klassik.pdf
```

## Contenuto

| Cartella | Descrizione |
|---|---|
| `notebooks/` | Notebook Jupyter con il codice di analisi e gli output già salvati |
| `corpus/` | Testi in formato EPUB (Schiller, Goethe, Lenz) |
| `docs/` | Relazione finale in PDF |

## Corpus

| Opera | Autore | Movimento |
|---|---|---|
| *Die Räuber* | Schiller | Sturm und Drang |
| *Götz von Berlichingen* | Goethe | Sturm und Drang |
| *Der Hofmeister* | J. M. R. Lenz | Sturm und Drang |
| *Iphigenie auf Tauris* | Goethe | Classicismo |
| *Maria Stuart* | Schiller | Classicismo |
| *Wallenstein* | Schiller | Classicismo |
