# acuris-orb-appgate

## Description
This orb installs the AppGate client and connects to our AppGate infra in AWS

## Authentication Setup
To get the connection to work you need the following
* CA cert from controller
* Username
* Password

These are stored in the AppGate context in our CircleCI setup
The CA cert is base64 encoded and setup as the APPGATE_CERT environment variable 
The username and password are in the appgate.conf file which has also been base64 encoded and stored as the APPGATE_CONF environment variable in the same AppGate context