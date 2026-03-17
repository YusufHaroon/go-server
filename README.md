# Go Server

A lightweight HTTP server built with **Golang** that demonstrates how to create and run a simple backend service using Go’s standard libraries.

This project serves as a **minimal starting point for building web servers or REST APIs in Go**. It shows how to handle HTTP requests, structure a basic Go application, and run a server locally.

---

## Features

- Lightweight HTTP server written in **Go**
- Simple routing and request handling
- Easy to extend for building APIs
- Minimal dependencies
- Beginner-friendly project structure

---

## Project Structure

```
go-server/
│
├── main.go        # Entry point of the server
├── go.mod         # Go module configuration
└── README.md      # Project documentation
```

---

## Prerequisites

Make sure you have the following installed:

- **Go (Golang)** – version 1.18 or higher  
- **Git**

Check your Go version with:

```bash
go version
```

If Go is not installed, download it from:  
https://go.dev/dl/

---

## Installation

Clone the repository:

```bash
git clone https://github.com/YusufHaroon/go-server.git
```

Navigate into the project directory:

```bash
cd go-server
```

---

## Running the Server

Run the server directly:

```bash
go run main.go
```

Or build and run the executable:

```bash
go build
./go-server
```

---

## Accessing the Server

Once the server starts, open your browser and go to:

```
http://localhost:8080
```

You should see the default response returned by the server.

---

## Example Endpoint

**GET /**

Response:

```
Hello World
```

---

## Development

To extend the server:

1. Add new routes in `main.go`
2. Implement handler functions
3. Restart the server

Example handler:

```go
func helloHandler(w http.ResponseWriter, r *http.Request) {
    fmt.Fprintf(w, "Hello from Go server!")
}
```
