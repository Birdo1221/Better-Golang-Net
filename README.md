# Go Ddos Botnet Controller

This project is a botnet controller implemented in Go (Golang) for managing bot connections and executing commands on connected bots over TCP/IP. 
This project is based on Network Overloading (Ddos) by sending overwhelming amount of traffic.

![Botnet Controller](https://github.com/Birdo1221/Better-Go-Cnc/assets/81320346/51845371-a14e-4581-865f-b5efba055a9d)

## Table of Contents

- [Overview](#overview)
- [Features](#features)
- [Setup](#setup)
- [Usage](#usage)
- [Contributing](#contributing)
- [License](#license)

## Overview

The Go Botnet Controller provides a server-client architecture where the server (controller) manages user connections and bot connections. Users can authenticate and interact with the botnet controller to send commands to connected bots.

The controller listens for connections on specified ports (`USER_SERVER_PORT` and `BOT_SERVER_PORT`) and handles incoming connections accordingly.

## Features

- User authentication system with username/password from a file (`users.txt`).
- Interactive command menu for users to view connected bots, view rules, send commands to bots, and view ongoing attacks.
- Handles concurrent connections using Goroutines.
- Basic bot command execution (`sendCommandToBots`) and management of ongoing attacks.

## Setup

1. **Clone Repository:**

   ```bash
   git clone https://github.com/Birdo1221/go-botnet-controller.git
   ```

2. **Navigate to Project:**

   ```bash
   cd go-botnet-controller
   ```

3. **Compile and Run:**

   ```bash
   go run main.go
   ```

## Usage

1. **Authentication:**

   - Connect to the controller using a TCP client (e.g., `telnet`).
   - Enter valid username and password to authenticate.

2. **Menu Options:**

   - `1`: View currently connected bots.
   - `2`: View rules and guidelines.
   - `3`: Send commands to connected bots.
   - `4`: View ongoing attacks.
   - `5`: Logout from the controller.

## Contributing

Contributions to this project are welcome. For major changes, please open an issue first to discuss what you would like to change.

1. Fork the repository.
2. Create your feature branch (`git checkout -b feature/your-feature`).
3. Commit your changes (`git commit -am 'Add some feature'`).
4. Push to the branch (`git push origin feature/your-feature`).
5. Open a pull request.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
