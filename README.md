# Prerequisites

Following software should be installed on your local machine:

- [.NET Core SDK 5.0](https://docs.microsoft.com/en-us/dotnet/core/install/)
- [Docker](https://docs.docker.com/) (optional)

# Getting started

These instructions will get you a copy of the projects up and running on your local machine for development and testing purposes.

## Running without docker

- Go to the folder `dotnetcore-template` with terminal und run these commands:
  `dotnet restore dotnet run`

- In browser go to `http://localhost:5000/WeatherForecast` or `https://localhost:5001/WeahterForecast` to see the api result

## Running with docker

1. Build image
   `sudo docker build -t dotnet-app . `
2. Run image
   `sudo docker run -p 3000:80 --name myfirstapp dotnet-app`
3. In browser go to `http://localhost:3000/WeatherForecast` to see the api result
