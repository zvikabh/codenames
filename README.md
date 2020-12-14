# Codenames Pictures

[![GoDoc](https://godoc.org/github.com/zvikabh/codenames?status.svg)](https://godoc.org/github.com/zvikabh/codenames)

This is a web app for generating and displaying boards for the <a href="https://en.wikipedia.org/wiki/Codenames_(board_game)">Codenames Pictures</a> board game. Generated boards are shareable and will update as words are revealed. The board can be viewed either as a spymaster or an ordinary player.

A hosted version of the app is available at [http://18.188.243.7](http://18.188.243.7).

![Screenshot of game board](https://raw.githubusercontent.com/zvikabh/codenames/master/screenshot.png)

### Building with Docker

The reposotiry includes a Dockerfile for building a docker image of this app.

```
docker build . -t codenames-pictures:latest
```

The following command will launch the docker image:

```
docker run --name codenames_server --rm -p 9091:9091 -d zvikabh/codenames-pictures
```

The following command will kill the docker instance:

```
docker stop codenames_server
```

## Credits

This is a fork from Jackson Owens's Codenames app, available on [https://github.com/jbowens/codenames](github.com/jbowns/codenames).
