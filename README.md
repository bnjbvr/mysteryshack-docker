### mysteryshack docker image (unofficial)

More information about mysteryshack [here](https://github.com/untitaker/mysteryshack).

- create a user:

```
d run -ti --rm \
    -v /path/to/config.ini:/rs/config.ini \
    -v /path/to/data:/rs/data \
    bnjbvr/mysteryshack \
    /rs/create-user.sh robert
```

- spawn a server:

```
d run -ti -d \
    -v /path/to/config.ini:/rs/config.ini \
    -v /path/to/data:/rs/data \
    -p 6767:6767 \
    bnjbvr/mysteryshack
```
