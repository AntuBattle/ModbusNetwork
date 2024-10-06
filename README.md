# ModBus Docker Network
This is an example of a Modbus Network developed using Docker contaienrs.
It has been utilized as a testbed for demonstration of vulnerabilities in the ModBus TCP/IP Protocol.

## Network Composition
The network is composed by a PLC (172.28.0.2), an HMI (172.28.0.5) and an intruder's PC (172.28.0.6), connected in the same internal network thanks to docker's 'bridge' network.

## Installation and Launch
To install and launch the project, just  ```cd ``` into the OT_Testbed_simulator and run
```bash
sudo docker compose up
```
