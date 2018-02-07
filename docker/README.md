# Logentries CLI Docker container
A simply container with lecli installed

## setup
`cp root/.config/config.ini.sample cp root/.config/config.ini`

then edit `root/.config/config.ini` and add your logentries api keys

## lecli arbitrary command
`docker-compose run --rm lecli lecli {lecli command args}`

## test if api keys are working
`docker-compose run --rm lecli lecli get apikeys`

## live tail
`docker-compose run --rm lecli letail {logs_name}`

## tested on
ubuntu 16.04 LTS

Docker version 17.05.0-ce, build 89658be

docker-compose version 1.17.1, build 6d101fb

