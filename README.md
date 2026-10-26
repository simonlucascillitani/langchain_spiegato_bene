# Python & LangChain spiegati bene

Il codice completo del libro **Python & LangChain spiegati bene** di Simonluca Scillitani, parte della Collana Tecnica AI & Systems.

Il libro insegna a costruire agenti con LangChain e LangGraph: dal primo agente fino a un sistema pronto per la produzione. Questo repository contiene tutto il codice che nel libro compare nei capitoli e nei laboratori, scaricabile e funzionante.

## A cosa serve

- Far girare sul tuo computer gli esempi di ogni capitolo senza ricopiare il codice dalla pagina.
- Fare i laboratori di fine capitolo (Test Lab) partendo da una traccia e confrontando il tuo lavoro con la soluzione completa.
- Avere sempre la versione aggiornata del codice, anche se hai la prima edizione del libro in Kindle o in cartaceo.

## Cosa trovi nel libro

Agenti con `create_agent`, tool, output strutturato, streaming, middleware, memoria, retrieval, grafi con LangGraph, persistenza e checkpoint, human-in-the-loop, multi-agente, tracing e valutazione con LangSmith, sicurezza e messa in produzione. Ogni capitolo ha un esercizio pratico basato su un caso reale.

## Come è organizzato il repository

Una cartella per capitolo, numerate da `capitolo-01` in poi. Dentro ogni cartella trovi sempre la stessa struttura:

```
capitolo-XX/
├── README.md          # cosa si fa nel capitolo e come eseguirlo
├── requirements.txt   # dipendenze con versioni esatte
├── .env.example       # variabili d'ambiente da copiare in .env
├── esempi/            # il codice mostrato nel capitolo
├── test-lab/
│   ├── traccia.md     # requisiti e traccia dell'esercizio
│   ├── soluzione/     # codice completo della soluzione
│   └── test/          # test che verificano la soluzione
└── sfida-extra/       # l'esercizio in più
```

## Requisiti

- Python 3.10 o superiore (è il requisito minimo del pacchetto `langchain`)
- Git
- La chiave API di un provider di modelli, solo per gli esempi che chiamano un modello reale

## Come si parte

```bash
git clone https://github.com/simonlucascillitani/langchain_spiegato_bene.git
cd langchain_spiegato_bene/capitolo-01

python -m venv .venv
source .venv/bin/activate      # su Windows: .venv\Scripts\activate
pip install -r requirements.txt

cp .env.example .env           # poi inserisci le tue chiavi in .env
```

Il file `.env` contiene le tue chiavi personali. Non va mai caricato su Git.

## Versioni

Il codice è scritto per la serie 1.x di LangChain. Ogni capitolo blocca le versioni esatte in `requirements.txt`, così il codice continua a funzionare anche quando le librerie escono in nuove versioni. Per ogni edizione del libro esiste un tag Git: se hai una copia stampata o digitale, usa il tag indicato nelle prime pagine del libro.

## Segnalare un errore

Se un esempio non gira o trovi una differenza tra libro e codice, apri una segnalazione nella sezione **Issues** del repository. Indica il capitolo, il sistema operativo e la versione di Python.

## Licenza

Il codice è distribuito con licenza **GPL-3.0**. Il testo completo è nel file [LICENSE](LICENSE). Il testo e le immagini del libro non sono coperti da questa licenza e restano di proprietà dell'autore.

## Autore

Simonluca Scillitani
