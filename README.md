# Go Botnet Controller

![Go Gopher](https://golang.org/doc/gopher/doc.png)

This project is a botnet controller implemented in Go (Golang) for managing bot connections and executing commands on connected bots over TCP/IP.

## Table of Contents

- ![Overview](https://example.com/overview.png) [Overview](#overview)
- ![Features](https://example.com/features.png) [Features](#features)
- ![Setup](https://example.com/setup.png) [Setup](#setup)
- ![Usage](https://example.com/usage.png) [Usage](#usage)
- ![Contributing](https://example.com/contributing.png) [Contributing](#contributing)
- ![License](https://example.com/license.png) [License](#license)

## Overview

![Controller Diagram](https://example.com/controller-diagram.png)

The Go Botnet Controller provides a server-client architecture where the server (controller) manages user connections and bot connections. Users can authenticate and interact with the botnet controller to send commands to connected bots.

The controller listens for connections on specified ports (`USER_SERVER_PORT` and `BOT_SERVER_PORT`) and handles incoming connections accordingly.

## Features

- ![Authentication](https://example.com/authentication.png) User authentication system with username/password from a file (`users.txt`).
- ![Menu](https://example.com/menu.png) Interactive command menu for users to view connected bots, view rules, send commands to bots, and view ongoing attacks.
- ![Concurrency](https://example.com/concurrency.png) Handles concurrent connections using Goroutines.
- ![Command Execution](https://example.com/command-execution.png) Basic bot command execution (`sendCommandToBots`) and management of ongoing attacks.

## Setup

1. **Clone Repository:**

   ```bash
   git clone https://github.com/your-username/go-botnet-controller.git
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

![Contributing](https://example.com/contributing-image.png)

Contributions to this project are welcome. For major changes, please open an issue first to discuss what you would like to change.

1. Fork the repository.
2. Create your feature branch (`git checkout -b feature/your-feature`).
3. Commit your changes (`git commit -am 'Add some feature'`).
4. Push to the branch (`git push origin feature/your-feature`).
5. Open a pull request.

## License

![License](https://example.com/license-image.png)

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
