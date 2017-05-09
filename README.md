# techo-nexus

To run, binding the exposed port 13020(YOURLOCALPORT) to the host.

```
$ docker run -d -p 13020:8081 --name nexus <<IMAGE_NAME>>
```

To (re)build the image:

Copy the Dockerfile and do the build-

```
$ docker build --rm=true nexus .
```

* It can take some time (2-3 minutes) for the service to launch in a
new container.  You can tail the log to determine once Nexus is ready:

```
$ docker logs -f nexus
```
