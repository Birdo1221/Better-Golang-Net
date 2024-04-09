# Botnet Controller and Botnet Client


![Botnet Controller](https://github.com/Birdo1221/Better-Go-Cnc/assets/81320346/51845371-a14e-4581-865f-b5efba055a9d)

This repository contains a botnet controller and a botnet client implemented in Go.

## Overview

The botnet controller manages user connections, handles bot commands, and orchestrates attacks on specified targets. The botnet client (bot) connects to the controller and executes commands received from it.

![Botnet Architecture](images/botnet_architecture.png)

## Botnet Controller

### Features:

- User authentication
- Menu-based user interface for command distribution
- Monitoring of ongoing attacks
- Rules enforcement for attack guidelines

### Usage:

1. Start the botnet controller server on the designated IP and port.
2. Connect clients (bots) to the controller.
3. Authenticate users to gain access to the controller's functionalities.
4. Use the menu to view connected bots, send commands, monitor ongoing attacks, and log out.

## Botnet Client (Bot)

### Features:

- HTTP, TCP, and UDP attack capabilities
- Duration-based attack execution
- Command interpretation from the controller
- STOP command handling for bot shutdown

### Usage:

1. Configure the bot with the controller's IP and port.
2. Connect the bot to the controller.
3. Receive commands from the controller to perform attacks.
4. Execute HTTP, TCP, or UDP attacks based on received commands.
5. Stop the bot on receiving the STOP command from the controller.

## Contributing

Contributions to this project are welcome. For major changes, please open an issue first to discuss what you would like to change.

1. Fork the repository.
2. Create your feature branch (`git checkout -b feature/your-feature`).
3. Commit your changes (`git commit -am 'Add some feature'`).
4. Push to the branch (`git push origin feature/your-feature`).
5. Open a pull request.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
