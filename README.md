# Botnet Controller and Botnet Client

This repository contains a botnet controller and a botnet client implemented in Go.
For Network overloading which can be used for Service Disruption. 

Please be aware that the Project provided here is intended for educational purposes only.
Legal Implications: Engaging in DDoS attacks is illegal in many jurisdictions and can result in serious legal consequences, including fines and imprisonment.

Ethical Concerns: Deliberately disrupting services or networks can harm innocent users and businesses, violating ethical principles of fairness and respect.

## Overview

The botnet controller manages user connections, handles bot commands, and makes attacks on specified targets. The botnet client (bot) connects to the controller and executes commands received from it.

## Botnet Controller

### Login Interface

![Botnet Controller Login](https://github.com/Birdo1221/Better-Go-Cnc/assets/81320346/0b125e4d-2b7d-431c-badc-a6555c2bb0f8)

### Main Interface

![Botnet Controller Main Interface](https://github.com/Birdo1221/Better-Go-Cnc/assets/81320346/51845371-a14e-4581-865f-b5efba055a9d)


### Features:

- User authentication Based On The Users.txt
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

### Installation and Running

#### 1. Install Go

First, ensure Go is installed on your system. You can download and install Go from the [official Go website](https://golang.org/dl/). Follow the installation instructions specific to your operating system.

#### 2. Set Up Botnet Controller

```bash
# Clone the botnet controller repository
git clone https://github.com/Birdo1221/Better-Go-Cnc.git

# Navigate to the controller directory
cd Better-Go-Cnc/controller

# Build and run the controller
go build ./controller
```

#### 2. Set Up Botnet Bot / Client

```bash
# Clone the botnet client repository
git clone https://github.com/Birdo1221/Better-Go-Cnc.git

# Navigate to the bot directory
cd Better-Go-Cnc/bot

# Build and run the bot
go build ./bot
```

## Future Development

The future development of this project may include:

- Improve How HTTP Read Its Received commands For Better Usage
- Adding additional attack methods
- Implementation of real-time attack monitoring and reporting
- Optimization for scalability and performance
- Client Security and Controller Security
- Safer Code and Clean-Up 

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
