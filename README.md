# python-web-api-bottle-basic-auth-ssl-sqlserver-ssl-simple

## Description
Creates an api of `dog` for a bottle project.
Has the ability to query by parameters.

Remotely tested with *testify*, the ssl is not verified.

Requires basic authentication for endpoints.

| username | password |
| -------- | -------- |
| *user* | *pass* |

Sql server uses self-signed ssl.

## Tech stack
- python
  - bottle
  - sqlalchemy
  - testify
  - requests
- mssql

## Docker stack
- alpine:edge
- python:latest
- mcr.microsoft.com/mssql/server:2017-CU17-ubuntu

## To run
`sudo ./install.sh -u`
- Get all pops: https://localhost/dog
  - Schema id, breed, and color
- CRUD opperations
  - Read: https://localhost/dog/<id> -u 'user:pass'

## To stop
`sudo ./install.sh -d`

## For help
`sudo ./install.sh -h`
