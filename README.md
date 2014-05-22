docker-mencached
---------------

Docker mencached server generic image source. This is based on `ubuntu:12.04` image.

Image
-----

You can `pull` a ready to use image from Docker
[index](https://index.docker.io/u/wiliamsouza/) running:

```
$ docker.io pull wiliamsouza/mencached
```

Or build this repository:

```
$ git clone https://github.com/wiliamsouza/docker-mencached.git
$ cd docker-mencached/
$ docker.io build -t wiliamsouza/mencached .
```

Change `wiliamsouza/mencached` to your Docker index username.

Container
---------

Shell access:

```
$ docker.io run -p 11211:11211 -i \
-t wiliamsouza/mencached /bin/bash
```

The command above will start a container give you a shell. Don't
forget to start the service running the `startup &` script.

Usage:

```
$ docker.io run --name mencached -p 11211:11211 -d \
-t wiliamsouza/mencached
```

The command above will start a container and return its ID.
