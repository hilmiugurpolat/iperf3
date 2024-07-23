# iPerf3 Usage Guide

This repository explains how to use iPerf3 in the command line.

## Installation

### 1. Clone the Repository

Clone the repository to your local machine using the following command:

```sh
git clone https://github.com/hilmiugurpolat/iperf3.git

**Server Mode**
To start iPerf3 in server mode, use the following command:
iperf3 -s

**Client Mode**
To start iPerf3 in client mode and connect to a server, use the following command:
iperf3 -c <server_ip_address>

**Basic Commands**
Here are some basic speed test commands using iPerf3:

Start server
iperf3 -s

Start client
iperf3 -c <server_ip_address>

**Example Commands**
To run a test for a specific duration (e.g., 60 seconds):
iperf3 -c <server_ip_address> -t 60

To specify a different port (default is 5201):
iperf3 -s -p 5001 # On the server
iperf3 -c <server_ip_address> -p 5001 # On the client

To run a bidirectional test (client to server and server to client):
iperf3 -c <server_ip_address> -d

To run a reverse test (server sends data to the client):
iperf3 -c <server_ip_address> -R
