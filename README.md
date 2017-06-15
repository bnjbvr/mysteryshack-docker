### mysteryshack docker image (unofficial)

More information about mysteryshack [here](https://github.com/untitaker/mysteryshack).

- first create a user (only need to do it once):

```
d run -ti --rm \
    -v /path/to/config.ini:/rs/config.ini \
    -v /path/to/data:/rs/data \
    bnjbvr/mysteryshack-docker \
    /rs/create-user.sh robert
```

- then spawn a server in the background:

```
d run -ti -d \
    -v /path/to/config.ini:/rs/config.ini \
    -v /path/to/data:/rs/data \
    -p 6767:6767 \
    bnjbvr/mysteryshack-docker
```
