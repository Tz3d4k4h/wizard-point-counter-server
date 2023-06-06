# Wizard-Point-Counter-Server

This repository stores the latest release of the server of the 
[Wizard-Point-Counter].
Furthermore, you find the docker infrastructure for deploying this server here.
The REST API of the server of the productive [Wizard-Point-Counter] can be 
accessed [here](https://wizardpointcounterservice-samueljonasgraf.b4a.run).

## Environment variables
In the environment, into which the server is deployed,
an environment variable called `DATABASE_URL` is required.
This variable configures the connection to the database used by the server
and has the following format:
```
postgres://${DATABASE_USER}:${DATABASE_PASSWORD}@${HOSTNAME}/${DATABASE_NAME}
```
In this format replace
* `${DATABASE_USER}`: with the user which shall be used for accessing the 
  database.
* `${DATABASE_PASSWORD}`: with the password for the user mentioned above.
* `${HOSTNAME}`: with the hostname of the database server of the used database.
* `${DATABASE_NAME}`: with the name of the used database.

[//]: # (TODO: Document api, e.g. with https://docs.rs/utoipa/latest/utoipa/)

[Wizard-Point-counter]: https://gitlab.com/Tzedakah/wizard-point-counter