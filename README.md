# Go Health Checker CLI

A simple command-line tool written in Go to check whether a website (or service) is **up or down** by attempting a TCP connection to a given domain and port.

## Features

- Check if a website is reachable
- Custom domain and port support
- Fast timeout-based TCP health check
- Simple CLI interface

## Installation

Make sure you have **Go 1.18+** installed.

Download dependencies:
go mod tidy

Usage

Run the tool using:
go run . --domain=google.com --port=443
OR
go run . -d google.com -p 443

Example Output

When the site is reachable:
[UP] google.com is reachable,
From: 192.168.1.5:51234
To: google.com:443

When the site is unreachable:
[DOWN] example.com is unreachable,
Error: dial tcp: lookup example.com: no such hos

Clone the repository:

```bash
git clone https://github.com/HarshDharmawat/healthcheck-cli.git
cd healthcheck-cli
