# FlexDXCluster

## Features

Program which connects to a DX cluster and sends the spots to a FlexRadio's panadapter after having check in Log4OM if entity has been already contacted, is a new band or new mode or both and sends the spot with different colors to Flex Panadapter. The program now comes with a user interface coded in Svelte and accessible through http://localhost:8080

Features:
- Can either auto discover Flex on the LAN or provide an IP address to connect to the radio
- Has a Telnet server included which replicates the DX spots received from the DX cluster client
- DX Cluster client which can connect to one of your prefered cluster
- Can send notification to Gotify for new entity, new band or new mode (can be disabled)
- Fill the callsign field in Log4OM when a spot is clicked on the Flex panadapter
- Sends the spot to the Flex Panadapter with different colors based on the status (new slot, new mode, new band, new band & mode, new dxcc, self spotted and so on...
- Now support any radio connected to CAT to Log4OM, every time a spot is clicked on the GUI, sends the call to Log4OM as well as Freq and Mode which should make the radio follow as well
- System of Watchlist to follow your prefered DX Expedition and tells on which slot you have not made the contact yet.

Any questions let me know

## How to Run the program

You need the .exe file, the config file (YAML format), update the config.yml to fit your needs and just run the .exe file and you are good to go.
Then connect with your web browser to http://localhost:8080

## Commands of the Telnet Server

The server running can manage the following commands:
- Bye
- DX (to send a spot)
- SH/DX xx
- SET/xxxx

All the commands will be forwarded to the DX Cluster server you are connected to.

73 de F4BPO
