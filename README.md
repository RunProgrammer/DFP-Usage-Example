# 🛰️ Data Flag Protocol (DFP)

The **Data Flag Protocol (DFP)** is a lightweight TCP-based client-server communication protocol designed for fast, structured, and optionally secure message exchange using predefined flags.


## 📌 Features
- Fixed-length header messaging
- Commands: `PING`, `SEND`, `RECEIVE`, `LOGIN`, `REGISTER`, `DISCONNECT`
- UTF-8 encoded messages with a delimiter
- SSL/TLS support (Comming soon)
- Logging on the server side
- Multi-threaded server handling concurrent clients


## 🧪 Supported Flags

| Flag       | Description                      |
|------------|----------------------------------|
| PING       | Check connection health          |
| SEND       | Send a message to the server     |
| RECEIVE    | Request a predefined message     |
| LOGIN      | Login with `username:password`   |
| REGISTER   | Register with `username:password`|
| DISCONNECT | Close the connection             |


## 📁 Folder Structure
.
├── server.py          # Server-side implementation of DFP
├── client.py          # Client-side interactive terminal interface
├── serverLog.log      # Auto-generated server log file
├── LICENSE            # Licensing information
└── README.md          # Project documentation



## 🛠️ Setup

Start the DFP server to begin accepting client connections. The server runs by default on `127.0.0.1:5000` 


### Server
```bash
python server.py (or)

python server.py --host 0.0.0.0 --port 8080

python client.py 

