# Atom on Docker

### Usage (manual)

```bash
xhost +
docker run -d -v /tmp/.X11-unix/:/tmp/.X11-unix/ \
              -v /dev/shm:/dev/shm \
              -v `pwd`:/workspace \
              -e DISPLAY=${DISPLAY} \
              fabert/docker-atom
```

```bash
xhost +
docker-compose run atom
```
