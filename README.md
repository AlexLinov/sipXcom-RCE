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

Run the script with the appropriate arguments.

![image](https://github.com/AlexLinov/sipXcom-RCE/assets/74632540/e0cd422c-2e03-44b1-8a31-41db9f042ac3)

## Credits

This script was inspired by an article on Packet Storm Security. You can read the full article [here](https://packetstormsecurity.com/files/171281/CoreDial-sipXcom-sipXopenfire-21.04-Remote-Command-Execution-Weak-Permissions.html).
