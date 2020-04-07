# Swagger generated server

## Overview
This server was generated by the [swagger-codegen](https://github.com/swagger-api/swagger-codegen) project. By using the
[OpenAPI-Spec](https://github.com/swagger-api/swagger-core/wiki) from a remote server, you can easily generate a server stub.

This example uses the [Connexion](https://github.com/zalando/connexion) library on top of Flask.

# Viewing API Specification
Please use the link to the .yaml swagger API specification file:

https://raw.githubusercontent.com/jackg-ch/swagger-user-api/master/swagger_server/swagger/swagger.yaml

The API documentation can be rendered in vscode or in the browser at https://editor.swagger.io/ by importing the above linked `swagger.yaml` file (File-->Import From URL)
## Requirements
Python 3.5.2+

## Usage
To run the server, please execute the following from the root directory:

```
pip3 install -r requirements.txt
python3 -m swagger_server
```

and open your browser to here:

```
http://localhost:8080/base/ui/
```

Your Swagger definition lives here:

```
http://localhost:8080/base/swagger.json
```

To launch the integration tests, use tox:
```
sudo pip install tox
tox
```

## Running with Docker

To run the server on a Docker container, please execute the following from the root directory:

```bash
# building the image
docker build -t swagger_server .

# starting up a container
docker run -p 8080:8080 swagger_server
```
