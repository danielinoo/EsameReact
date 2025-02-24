# React Native progetto Volo

Sito voli è un'applicazione React Native che consente agli utenti di cercare voli, visualizzare aeroporti e compagnie aeree. L'app si collega a un backend Flask per recuperare i dati che stanno dentro un file json.

# Funzionalità
- **Ricerca Volo**: L'utente può cercare voli inserendo aeroporto di partenza e di arrivo.
    -**risultato negativo**:
        Se non ci sono voli disponibili per la sua richesta mostrerà a schermo " AL MOMENTO NON CI SONO VOLI PER QUESTA TRATTA" se invece
    -**risultato positivo**:
        Se ci sono voli per la sua richiesta mostrerà una tabella con i voli specifici per la sua tratta 
- **Visualizzazione Aeroporti**: Mostra l'elenco degli aeroporti disponibili.
- **Visualizzazione Compagnie Aeree**: Lista delle compagnie aeree con i relativi dettagli.
- **Visualizzazione Voli**: Elenco completo dei voli con informazioni su partenza, arrivo e orari.

# Tecnologie Utilizzate

- **Frontend**: React Native (con `react-native-web` per supporto web)
- **Backend**: Flask (API REST per la gestione dei dati)
- **HTTP Client**: Axios (per le richieste al server)
- **UI & Stile**: `react-native`, `react-native-web`, `react-native-safe-area-view`



## Installazione e Avvio

### Requisiti
- **Node.js** e **npm** per il frontend
- **Python** e **Flask** per il backend

###  Clonare il repository
```sh
git clone https://github.com/danielinoo/EsameReact.git
```
```sh
cd ProgettoReactNative_cielo
```

### Avvio del backend
1. Installare Flask e le dipendenze:
   ```bash
   pip install flask flask-cors
   ```
2. Eseguire il server Flask:
   ```bash
   python server_json.py
   ```
Il backend sarà attivo su `http://127.0.0.1:5004`.

### Avvio del frontend
1. Dentro la cartella del frontend:
   ```bash
    nvm install node
   ```
2. Installare le dipendenze:
   ```bash
   npm install
   ```
3. Avviare l'app ProgettoReactNative_cielo:
   ```bash
   npm run web
   ```
   (oppure npm run android / npm run ios)











