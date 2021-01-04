# portscanner
Port Scanner using Python and Flask as framework with JWT Authentication and MongoDB

This is an API only project that after authentication takes in an IP or Domain as an input and provides a unique scan ID to lookup open port results from the database later.

Plan is to create a webhook that will call any API once the port scanning is done. This is going to be a living documentation.

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

Attached postman collection should help find the APIs
