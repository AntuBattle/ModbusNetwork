# ModBus Docker Network
This is an example of a Modbus Network developed using Docker contaienrs.
It has been utilized as a testbed for demonstration of vulnerabilities in the ModBus TCP/IP Protocol.

## Network Composition
The network is composed by three containers: a PLC (172.28.0.2), an HMI (172.28.0.5) and an intruder's PC (172.28.0.6) called attacker, connected in the same internal network thanks to docker's 'bridge' network.

## PLC Monitoring Interface
A PLC Monitoring interface is available by default at $\texttt{localhost:8080}$, accessible using default credentials 'openplc' as both username and password.
From there, it is possible to monitor the status of the configured PLC memory addresses (3 coils up to now) and upload scripts for the PLC to execute, among other things.

## Installation and Launch
To install and launch the project, just  ```cd``` into the OT_Testbed_simulator directory and run
```bash
sudo docker compose up
```
