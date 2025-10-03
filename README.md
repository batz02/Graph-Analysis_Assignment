
# README

## Descrizione

Questo progetto analizza la rete dei voli usando tecniche di graph analytics in Python e Neo4j.  
Il file principale è `GA_flight.ipynb`.

---

## Requisiti

- Python 3
- Jupyter Notebook
- Neo4j Desktop
- Pacchetti Python: `pandas`, `networkx`, `matplotlib`, `py2neo`, `neo4j`

---

## 1. Avvio Notebook

1. Apri il terminale nella cartella del progetto.
2. (Opzionale) Crea un ambiente virtuale:
   ```bash
   python3 -m venv venv
   source venv/bin/activate```    

3. Installa i pacchetti necessari:

   ```bash
   pip install pandas networkx matplotlib py2neo neo4j notebook```
4. Avvia Jupyter:

   ```bash
   jupyter notebook
   ```
5. Apri il file `GA_flight.ipynb` dal browser.

---

## 2. Installazione e avvio Neo4j Desktop

1. Scarica e installa [Neo4j Desktop](https://neo4j.com/download/).
2. Crea un nuovo progetto e all’interno crea un nuovo database (puoi chiamarlo come preferisci).
3. Avvia il database cliccando su “Start”.
4. Installa il plugin **Graph Data Science** dal pannello “Plugins” (è sufficiente cliccare su “Install”).
5. Prendi nota di:

   * **Username** (di default `neo4j`)
   * **Password** (ti viene chiesto di sceglierla al primo avvio)
   * **Bolt URI** (di solito `bolt://localhost:7687`)

---

## 3. Configura il notebook

All’inizio del file `GA_flight.ipynb`, controlla che questi parametri siano corretti in base al tuo setup Neo4j:

```python
NEO4J_URI = "bolt://localhost:7687"
NEO4J_USER = "neo4j"
NEO4J_PASS = "password"
```

---

## 4. Dati

Assicurati che i file dei dati (esempio: `airports.csv`, `routes.csv`) siano nella **stessa cartella** del notebook `GA_flight.ipynb`.

---

## 5. Esecuzione

Segui le celle del notebook `GA_flight.ipynb` passo passo.

* Le query Cypher per importare i dati e analizzarli sono già incluse nel notebook.
* Prima di eseguire le parti che usano Neo4j, assicurati che il database sia avviato.
---