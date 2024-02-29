
# Man-in-the-Middle Attack Simulation (icscw2)

This repository features a simulation for UoE's 'Introduction to Computer Security' course, showcasing a man-in-the-middle (MITM) attack on the Diffie-Hellman protocol. It demonstrates how an attacker can intercept and alter the public keys between two parties, Alice and Bob, to decrypt and potentially modify their messages by establishing a shared secret key with each. 

## Features

- **Diffie-Hellman Key Exchange**: Implements the Diffie-Hellman key exchange protocol, allowing two parties to establish a shared secret key over an insecure channel.
- **AES Encryption**: Uses AES encryption in CTR mode for encrypting and decrypting messages between Alice and Bob.
- **UNIX Socket Communication**: Utilizes UNIX sockets for inter-process communication between Alice and Bob.
- **Simple User Interface**: Includes a basic text-based user interface for interacting with the chat system.
- **MITM Attack Simulation**: Demonstrates how an attacker can intercept and potentially alter the messages exchanged between Alice and Bob during the key exchange phase.

## Getting Started

1. **Clone the Repository**: Clone this repository to your local machine.
2. **Install Dependencies**: Ensure you have Python installed on your machine. This project uses standard Python libraries, so no additional dependencies are required.
3. **Run the Simulation**: Navigate to the project directory and run the main script with the player name as an argument. For example, to simulate Alice's side, run `python simple_sockets.py alice`.

## Usage

- **Alice and Bob**: Run the simulation in two separate terminals, one for Alice and one for Bob, using the command `python simple_sockets.py <player_name>`, where `<player_name>` is either `alice` or `bob`.
- **Attacker**: The attacker's role is simulated by intercepting and potentially altering the messages exchanged between Alice and Bob during the key exchange phase. This is demonstrated in the `simple_sockets.py` and `util.py` files.
