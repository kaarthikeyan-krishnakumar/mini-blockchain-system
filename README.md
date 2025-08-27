# Mini Blockchain System

A lightweight blockchain implementation in Python using Flask.
This project demonstrates how blockchain works through block mining, proof of work, transaction handling, and chain validation — all accessible via REST API endpoints.

---

## Features

• Add new transactions
• Mine blocks using Proof of Work
• Retrieve the full blockchain
• Validate the blockchain integrity

---

## Tech Stack

• Python 3
• Flask (API framework)
• PowerShell / cURL / Postman (API testing)

---

## Project Structure

blockchain.py        - Core blockchain logic
blockchain\_app.py    - Flask server and API routes
images/              - Screenshots (API testing, server logs)
README.md            - Project documentation

---

## Quick Start

1. Clone the repository
   git clone [https://github.com/your-username/mini-blockchain-system.git](https://github.com/your-username/mini-blockchain-system.git)
   cd mini-blockchain-system

2. Install dependencies
   pip install flask

3. Run the Flask server
   python blockchain\_app.py

Server runs at:
[http://127.0.0.1:5000/](http://127.0.0.1:5000/)
[http://192.168.xxx.xxx:5000/](http://192.168.xxx.xxx:5000/) (local network access)

---

## API Endpoints

POST   /add\_transaction     -> Add a new transaction
GET    /mine\_block          -> Mine a block and add it to the chain
GET    /get\_chain           -> Retrieve the full blockchain
GET    /is\_valid            -> Check blockchain validity

Example:
POST /add\_transaction
{ "sender": "Alice", "receiver": "Bob", "amount": 10 }

---

## How It Works

1. Start the Flask server
2. Add transactions through the API
3. Mine blocks to include transactions
4. Validate the chain to ensure immutability

---

## Future Enhancements

• Peer-to-peer node connections
• Consensus mechanism for distributed blockchain
• Web-based user interface

---

## Screenshots

(output images/all_endpoints_output.jpg)
(output images/flask_server_logs.jpg)

---