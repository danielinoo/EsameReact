# React + Vite Gestione Voli


Gestione Voli è un'applicazione web per la gestione dei voli, delle compagnie aeree e degli aeroporti. Comprende una parte frontend sviluppata in **React** e una parte backend realizzata con **Flask**.

## Struttura del Progetto

### Frontend (React)
Il frontend dell'applicazione fornisce un'interfaccia per la ricerca e visualizzazione dei voli, delle compagnie e degli aeroporti.

- **Home.jsx**: Pagina principale con un messaggio di benvenuto.
- **Navbar.jsx**: Barra di navigazione con i collegamenti alle diverse sezioni dell'app.
- **RicercaVolo.jsx**: Permette di cercare voli inserendo aeroporto di partenza e arrivo, se non sono presenti i voli richiesti restituirà il mesaggio "AL MOMENTO NON CI SONO VOLI PER QUESTA TRATTA".
- **Vis_volo.jsx**: Visualizza l'elenco dei voli disponibili.
- **Vis_com.jsx**: Visualizza l'elenco delle compagnie aeree.
- **Vis_Aer.jsx**: Visualizza l'elenco degli aeroporti.

### Backend (Flask)
Il backend fornisce le API per recuperare e gestire i dati relativi ai voli, compagnie e aeroporti.

- **server_json.py**: Contiene tutte le route per gestire le richieste al server.
  - `GET /voli` → Restituisce l'elenco dei voli.
  - `GET /visualizza_aeroporti` → Restituisce l'elenco degli aeroporti.
  - `GET /visualizza_compagnie` → Restituisce l'elenco delle compagnie.
  - `POST /RicercaVolo` → Restituisce i voli che corrispondono ai criteri di ricerca.
- **database.json**: Contiene i dati dei voli, compagnie e aeroporti.

## Installazione e Avvio

### Requisiti
- **Node.js** e **npm** per il frontend
- **Python** e **Flask** per il backend

###  Clonare il repository
```sh
git clone https://github.com/danielinoo/EsameReact.git
```
```sh
cd ProgettoReact_cielo
```

### Avvio del backend
1. Installare Flask e le dipendenze:
   ```bash
   pip install flask flask-cors
   ```
2. Eseguire il server Flask (dentro SRC):
   ```bash
   python server_json.py
   ```


### Avvio del frontend
1. Dentro la cartella del frontend:
   ```bash
    nvm install node
   ```
2. Installare le dipendenze:
   ```bash
   npm install
   ```
3. Avviare l'app ProgettoReact_cielo:
   ```bash
   npm run dev
   ```


## Tecnologie Utilizzate
- **Frontend**: React.js, React Router
- **Backend**: Flask, Flask-CORS
- **Database**: JSON file per la gestione dei dati



