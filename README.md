# FlexDXCluster

## Features

Program which connects to a DX cluster and sends the spots to a FlexRadio's panadapter after having check in Log4OM if entity has been already contacted, is a new band or new mode or both and sends the spot with different colors to Flex Panadapter.

Features:
- Can either auto discover Flex on the LAN or provide an IP address to connect to the radio
- Has a Telnet server included which replicates the DX spots received from the DX cluster client
- DX Cluster client which can connect to one of your prefered cluster
- Can send notification to Gotify for new entity, new band or new mode (can be disabled)
- Fill the callsign field in Log4OM when a spot is clicked on the Flex panadapter
- Sends the spot to the Flex Panadapter

If you do not use Log4OM but still use a program with SQLite database or MySQL it should work if the db name is "log".

Any questions let me know

## How to Run the program

You need the .exe file, the config file (YAML format) and the country.xml, update the config.yml to fit your needs and just run the .exe file and you are good to go.

## Commands of the Telnet Server

The server running can manage the following commands:
- Bye
- DX (to send a spot)
- SH/DX xx

All the commands will be forwarded to the DX Cluster server you are connected to.

73 de F4BPO
