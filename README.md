# portscanner
Port Scanner using Python and Flask as framework with JWT Authentication and MongoDB

This is an API only project that after authentication takes in an IP or Domain (can also process multiple IPs and Domains) as an input and provides a unique scan ID to lookup open port results from the database later.

# SETUP:

Clone the project
Add in mongo_string.text to provide database credentials
Add in secret_key.txt to provide a salt to the JWT encoding
Download and Install Docker using the link shown below:
https://docs.docker.com/get-docker/
Install Docker Compose:
https://docs.docker.com/compose/install/

CD into the cloned directory and type docker-compose up and press enter

This should build/pull the images required to run the project. Portscanner will be available on http://0.0.0.0:5000

# Attached postman collection to repo which should help test the APIs

Future Plans:

- Adding a webhook option that would call the given API after the scanning is complete
- Adding an ssl cert check API that would return expiry and start dates along with other host specific data
- Adding a new API that would port scan a CIDR block
- Expanding beyond just open ports to guessing what OS is being used, etc on the host system
