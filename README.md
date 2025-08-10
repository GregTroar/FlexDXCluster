# FlexDXCluster

## Features

Program which connects to a DX cluster and sends the spots to a FlexRadio after having check in Log4OM if entity has been already contacted, is a new band or new mode or both and sends the spot with different colors to Flex Panadapter.

Features:
- Can either au to discover Flex on the LAN or provide an IP address to connect to the radio
- Has a Telnet server included which replicates the DX spots received from the DX cluster client
- DX Cluster client which can connect to one of your prefered cluster
- Can send notification to Gotify for new entity, new band or new mode (can be disabled)
- Fill the callsign field in Log4OM when a spot is clicked on the Flex panadapter

If you do not use Log4OM but still use a program with SQLite database or MySQL it should work if the db name is "log".

Any questions let me know

## How to Run the program

You need the .exe file, the config file (YAML format) and the country.xml, just run the .exe file and you are good to go.

73 de F4BPO
