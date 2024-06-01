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

This option retrieves logs from the server. Start a netcat listener on port 80 to retrieve the logs.

```bash
python3 poc_script.py --help
```
