# megatools-docker
Docker image for running megatools.  
This image builds the current version of meatools from github source

## Pull from dockerhub
* https://hub.docker.com/r/aenygma/megatools
* `docker pull aenygma/megatools`

## Configs
By default files will be downloaded to `~/Downloads/mega_dls`.  
This can be configured in `mega.sh` via variable `DUMP_DIR`

Megatools config (`.megarc`) can be added to the current directory for convenience.  
(See https://megatools.megous.com/man/megarc.html)
Typically useful for username/password and transfer configs

## Usage

Source the sh helpers
```
. mega.sh
```

Build the container
```
dbuild
```

Download a Mega url
```
megadl <url>
```

Unload the sh helpers
```
deactivate
```
