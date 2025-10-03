
## Description

This project analyzes the flight network using graph analytics techniques in Python and Neo4j.  
The main file is `GA_flight.ipynb`.


## Requirements

- Python 3
- Jupyter Notebook
- Neo4j Desktop
- Python packages: `pandas`, `networkx`, `matplotlib`, `py2neo`, `neo4j`


## 1. Starting the Notebook

1. Open the terminal in the project folder
2. (Optional) Create a virtual environment:

```
python3 -m venv venv
source venv/bin/activate
```

3. Install the required packages:
```
pip install pandas networkx matplotlib py2neo neo4j notebook
```

4. Start Jupyter:
```
jupyter notebook
```
5. Open the `GA_flight.ipynb` file from the browser


## 2. Installing and Starting Neo4j Desktop

1. Download and install [Neo4j Desktop](https://neo4j.com/download/)
2. Create a new project and inside it create a new database (you can name it as you like)
3. Start the database by clicking "Start"
4. Install the **Graph Data Science** plugin from the "Plugins" panel (just click "Install")
5. Take note of:

* **Username** (default is `neo4j`)
* **Password** (you will be asked to set it at the first start)
* **Bolt URI** (usually `bolt://localhost:7687`)


## 3. Configure the notebook

At the beginning of the `GA_flight.ipynb` file, check that these parameters are correct according to your Neo4j setup:
```
NEO4J_URI = "bolt://localhost:7687"
NEO4J_USER = "neo4j"
NEO4J_PASS = "password"
```

## 4. Data

Make sure the data files (example: `airports.csv`, `routes.csv`) are in the **same folder** as the `GA_flight.ipynb` notebook.


## 5. Execution

Follow the cells in the `GA_flight.ipynb` notebook step by step.

* The Cypher queries to import and analyze data are already included in the notebook.
* Before running parts that use Neo4j, make sure the database is running.
