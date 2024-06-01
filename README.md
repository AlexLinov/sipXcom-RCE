# XMPP Exploit PoC Script

This repository contains a Python script to exploit vulnerabilities in sipXopenfire, specifically for the following CVEs:
- CVE-2023-25355
- CVE-2023-25356

The script allows for two types of payloads:
1. Retrieve logs from the server.
2. Overwrite the Openfire configuration to include a reverse shell.

## Requirements

- Python 3.x
- `xmpppy` library

```bash
pip install xmpppy
```
## Usage

Run the script with the appropriate arguments. The available options are described below:

### Retrieve Logs

Payload option 1 retrieves logs from the server. Start a netcat listener on port 80 to retrieve the logs.

### Overwrite Openfire Configuration for Reverse Shell

Payload option 2 overwrites the Openfire configuration to include a reverse shell. You need to provide a file to serve for the reverse shell. The script will start a Python HTTP server on the specified port (default is 8080) to serve the file. See `openfire.txt` file

```bash
python3 poc_script.py --help
```
## Credits

This script was inspired by an article on Packet Storm Security. You can read the full article [here](https://packetstormsecurity.com/files/171281/CoreDial-sipXcom-sipXopenfire-21.04-Remote-Command-Execution-Weak-Permissions.html).
