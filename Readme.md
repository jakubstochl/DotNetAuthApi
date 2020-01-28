# NotesApi application

Basic tutorial to show creation of JWT token in REST API

Disclaimer:
Application is just for educational purposes, does not contain proper error handling, logging etc.

## Getting Started

These instructions will get you a copy of the project up and running on your local machine.

### Prerequisites

Development of application requires following software to be installed:
* Visual Studio Code or other C# .net project editor.
* .net core 3.1 SDK (https://dotnet.microsoft.com/download/dotnet-core/3.1)
* Docker (if you wish to run application in container)

### Installing

* Clone repository.
* Run command dotnet restore.

#### Running directly

* Execute command dotnet run
* Check that application is running on given url and port by calling curl.

#### Running in docker

Use docker-compose up to start application in container.

## Exposed APIs and example of calls
    
    curl --location --request POST 'http://localhost:5000/auth/authenticate' \
        --header 'Content-Type: application/json' \
        --data-raw '{
	        "username" : "test",
	        "password" : "test"
    }'

