# Hypertext Transfer Protocol

How to build an HTTP client-server model using Bottle, Requests, and cURL. We'll create CRUD APIs for managing a shopping list, allowing you to create, read, update, and delete products.

## API Specification

| **Method** | **Pathname**           | **Body Type** |
|------------|------------------------|---------------|
| POST       | `/products`            | JSON          |
| GET        | `/products`            | -             |
| PUT        | `/products/{product}`  | Plain Text    |
| DELETE     | `/products/{product}`  | -             |

---

# HTTP Overview

The **Hypertext Transfer Protocol (HTTP)** is a web application-layer protocol that implements the client-server model:

- The client requests, receives, and "displays" web objects.
- The server sends objects in response to requests.

### How HTTP Works:
- An HTTP client initiates a **TCP connection** (creates a socket) to the server, typically over port 80.
- The server accepts the TCP connection from the client.
- The hosts exchange HTTP messages before closing the TCP connection.

---

## Install Requirements

To set up the project environment, follow these steps to create a virtual environment and install the required dependencies:

```bash
sudo pip3 install virtualenv
virtualenv -p python3 venv
source venv/bin/activate
pip install -r requirements.txt
