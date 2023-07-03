# Nginx Mocker

`nginx-mocker` is a convenient utility designed to simulate the default NGINX web page. Whether you're a developer needing to test applications against an NGINX response, or you're learning about client-server interactions, `nginx-mocker` provides a quick and easy way to mimic an NGINX server behavior. This utility is written in Rust and uses Hyper, an HTTP library for Rust, to create a server that listens to requests and responds with the default NGINX page.

## Features

- Returns the default NGINX web page on GET requests to the root ("/") endpoint.
- Lightweight and easy to use.
- No need to set up complex NGINX infrastructure.

## Getting Started

To use `nginx-mocker`, you'll need to have Rust installed on your machine.

1. Clone this repository:
```
git clone https://github.com/wiresock/nginx-mocker.git
```

2. Navigate to the project directory:
```
cd nginx-mocker
```

3. Build and run the application:
```
cargo build
cargo run
```
or you can specify the port number when you run the application:
```
cargo run <port_number>
```

The server will start and listen for incoming connections. Press ENTER to exit the server.

## Usage

Once the server is running, simply make a GET request to `http://localhost:<port_number>/` to receive the default NGINX page.

For example, using curl:
```
curl http://localhost:<port_number>/
```
