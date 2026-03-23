# Flask Blockchain Simulation

This is a simple **Blockchain Simulation** built with **Python** and **Flask**.  
It demonstrates how a blockchain works by creating **5 blocks** with transactions and showing them on a **webpage**.

---

## Features

- ✅ **Genesis Block** creation  
- ✅ **5 Blocks** with sample transactions:
  1. Alice pays Bob 10 BTC  
  2. Bob pays Charlie 5 BTC  
  3. Charlie pays Dave 2 BTC  
  4. Dave pays Eve 1 BTC  
  5. Eve pays Alice 0.5 BTC  
- ✅ Each block contains:
  - Index (block number)  
  - Timestamp  
  - Data (transaction info)  
  - Previous block’s hash  
  - Current block hash  
- ✅ Display all blocks in a **browser** using Flask and HTML  

---

## Installation

1. Clone the repository:

```bash
git clone https://github.com/yourusername/flask-blockchain.git
cd flask-blockchain
```

2. Install dependencies:

```bash
pip install flask
```

---

## Usage

1. Run the Flask app:

```bash
python app.py
```

2. Open your browser and go to:

```
http://127.0.0.1:5000/
```

3. You will see all 5 blocks displayed with their details.

---

## Project Structure

```
BlockchainProject/
│
├─ app.py               # Main Flask application
├─ README.md            # Project README
├─ templates/
│   └─ index.html       # HTML template to display blocks
```

---

## How It Works

- The **Genesis Block** is created first with a previous hash of "0".  
- Each new block stores:
  - A transaction (`data`)
  - A timestamp
  - The previous block's hash
  - Its own hash generated using **SHA-256**  
- Flask renders all blocks on the homepage using **Jinja2 templates**.

---

## License

This project is **open-source** and free to use.
