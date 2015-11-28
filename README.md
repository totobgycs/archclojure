# archclojure
Archlinux docker image with Clojure, Eclipse and Counterclockwise based on [totobgycs/archjava](https://registry.hub.docker.com/u/totobgycs/archjava/).
It contains [Clojure](clojure.org), [Leiningen](leiningen.org) and [Counterclockwise](http://www.ccw-ide.org/). 

Usage:

```
$ xhost +si:localuser:eclipse
$ docker run -d -e DISPLAY -v /tmp/.X11-unix:/tmp/.X11-unix:ro totobgycs/archclojure eclipse
```

or

```
$ xhost +si:localuser:eclipse
$ docker run -it -e DISPLAY -v /tmp/.X11-unix:/tmp/.X11-unix:ro totobgycs/archclojure /bin/bash
```

and then start eclipse from the command prompt.
