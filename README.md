# minecraft-server
A Minecraft Server Docker Container

## Description
This is a Minecraft server with a host mountable data directory. It is based off the alpine official image and openjdk8.

## Installation/Running Container
To run this container:

```bash
docker run -d --name mc1 -v /hostdatadir:/data -p 25565:25565 moutansos/minecraft-server
```

## Logs

Server logs are kept at:
```bash
/hostdatadir/server.log
```

## Configuration

Server config files are found in the host data directory
