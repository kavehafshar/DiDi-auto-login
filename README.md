# DiDi WiFi Auto Login Script

A Bash script that automatically authenticates you on the DiDi-UK WiFi network when connected.

## Table of Contents
- [Features](#features)
- [Prerequisites](#prerequisites)
- [Installation](#installation)
- [Configuration](#configuration)
- [Usage](#usage)


## Features

- Automatically detects when connected to "DiDi-UK" WiFi
- Handles the authentication process without browser interaction
- Lightweight (under 10 lines of active code)
- Works with standard Linux network utilities

## Prerequisites

- Linux distribution with NetworkManager (most Ubuntu/Debian/Fedora installations)
- `curl` for HTTP requests (install with `sudo apt install curl` if missing)

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/kavehafshar/DiDi-auto-login.git
   cd DiDi-auto-login
   
2. Make the script executable:
   ```bash
   chmod +x didi-wifi-login.sh
   
   
## Configuration

1. Edit the script with your credentials:
    ``` bash
    nano didi-wifi-login.sh


2. Find these lines and insert your DiDi WiFi credentials:
    ``` bash
    USERNAME="your_didi_username"  # Replace with your actual username
    PASSWORD="your_didi_password"  # Replace with your actual password

Save the file (Ctrl+O, then Ctrl+X in nano).


## Usage

1. Automatic Login Method,
 NetworkManager Dispatch Script

    ```bash
    sudo cp didi-wifi-login.sh /etc/NetworkManager/dispatcher.d/99-didi-login.sh

This will run automatically whenever your network connection changes.

2. Manual Execution,
Run the script directly:

    ```bash
    ./didi-wifi-login.sh


    
