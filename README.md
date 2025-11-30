# 📡 Computer Networks Lab

## 📘 Overview
This repository contains practical implementations of fundamental computer networking concepts using **C** and **Python**. Each lab focuses on building real-world components such as TCP clients/servers, multithreaded systems, and a minimal HTTP webserver. These exercises are designed to strengthen understanding of network protocols, socket communication, and concurrency.

---

## 🧪 Projects

### 🔹 Lab 1: Basic Client-Server Communication
**Objective:** Implement a simple TCP-based interaction between a client and a server.  
**Languages:** C, Python  

**Key Concepts:**
- Creating and binding sockets  
- Listening for client connections  
- Sending and receiving messages  
- Basic request–response flow  

---

### 🔹 Lab 2: Multithreaded Server with Client Simulation
**Objective:** Build a multithreaded server that can handle multiple clients at the same time.  
**Languages:** C, Python  

**Key Concepts:**
- Creating and managing threads  
- Concurrent client handling  
- Simulating multiple clients on one machine  
- Synchronization and safe shared data handling  

---

### 🔹 Lab 3: Webserver (Socket Programming in C)
**Objective:** Develop a basic webserver in C that processes HTTP GET requests and serves an `index.html` file.  
**Languages:** C  

**Key Concepts:**
- TCP socket creation  
- Port binding and listening (e.g., port 8080)  
- Accepting browser connections  
- Parsing HTTP request headers  
- Sending HTTP response headers + HTML content  
- Packet inspection using Wireshark  

---

## 📝 Steps

- Create an HTML file named **index.html** to serve.  
- Implement **webserver.c** to handle socket communication:  
    - Wait for HTTP GET requests.  
    - Send back HTTP 200 OK header + contents of index.html.  
- Compile and run the server:  
    ```bash
    gcc webserver.c -o webserver
    ```
- Run server:  
    ```bash
    ./webserver
    ```
- Open a browser and visit:  
    ```
    http://localhost:8080
    ```
- You should see the contents of `index.html`.  
- Use **Wireshark** to capture and analyze packets:  
    - Observe TCP three-way handshake.  
    - Inspect the HTTP GET request sent by the browser.  
    - Inspect the HTTP response containing the HTML page.

**Features:**  
- Serves static HTML content  
- Minimal and readable HTTP handling  
- Demonstrates browser ↔ TCP server communication  

---

## 🚀 Getting Started

### Prerequisites

#### C
- GCC  
- pthread library  

#### Python
- Python 3.x  
- `socket` library (built-in)  

---

## ⚙️ Compilation and Execution

### C Implementation
- Compile server:  
    ```bash
    gcc server.c -o server -pthread
    ```
- Run server:  
    ```bash
    ./server
    ```
- Compile client:  
    ```bash
    gcc client.c -o client
    ```
- Run simulated clients:  
    ```bash
    ./client 1
    ./client 2
    ```

---

## 🌟 Features Across Labs
- Fully working multithreaded servers  
- Simulation of multiple clients on one machine  
- Client/Server implementations in both C and Python  
- Webserver capable of serving real HTML files  
- Wireshark packet-level analysis  
- Modular structure — each lab is standalone
