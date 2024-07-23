# iPerf3 Usage Guide

This repository explains how to use iPerf3 in the command line.

## Installation

### 1. Clone the Repository

Clone the repository to your local machine using the following command:

git clone https://github.com/hilmiugurpolat/iperf3.git

## Usage

**Server Mode**

To start iPerf3 in server mode, use the following command:
 ```sh
iperf3 -s
 ```
**Client Mode**

To start iPerf3 in client mode and connect to a server, use the following command:
  ```sh
iperf3 -c <server_ip_address>
```
**Basic Commands**

**Start Server**
 ```sh
iperf3 -s
 ```
**Start Client**

1. **Clone the repository:**

    ```sh
   iperf3 -c <server_ip_address>

    ```

**Example Commands**

**Run a Test for a Specific Duration (e.g., 60 seconds)**
 ```sh
iperf3 -c <server_ip_address> -t 60
```

**Specify a Different Port (default is 5201)**

On the server:
 ```sh
iperf3 -s -p 5001
 ```
On the client:
 ```sh
iperf3 -c <server_ip_address> -p 5001
 ```
**Run a Bidirectional Test (client to server and server to client)**
 ```sh
iperf3 -c <server_ip_address> -d
```
**Run a Reverse Test (server sends data to the client)**
```sh
iperf3 -c <server_ip_address> -R
```
