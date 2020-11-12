# Ca_Server
The Ca Server provides an API to issue and revoke user certificates.

## Installation
Use the packet manager to install the following packets:

```bash
pip install flask base 64 enum random os json argparse
```
## Usage
First set up the chain of trust by running the following command. As SECRET you should provide a password to encrypt the private key of the root CA.

```bash
./set_up_ca.sh root.cnf intermediate.cnf <SECRET>
```

Start the API with the following command

```bash
python3 ca_app.py
```
