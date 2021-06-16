# Containerize a .NET Core app

## Essential commands
### docker build -t counter-image -f Dockerfile .
### docker create --name core-counter counter-image
### docker start core-counter
### docker attach --sig-proxy=false core-counter
### docker stop core-counter

## Single run
### docker run -it --rm counter-image 3

## Changing Entrypoint
### docker run -it --rm --entrypoint "bash" counter-image