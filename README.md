### mysteryshack docker image (unofficial)

- create a user:

```
d run -ti --rm \
    -v /path/to/config.ini:/rs/config.ini \
    -v /path/to/data:/rs/data \
    bnjbvr/mysteryshack \
    mysteryshack user create robert
```

- spawn a server:

```
d run -ti --rm \
    -v /path/to/config.ini:/rs/config.ini \
    -v /path/to/data:/rs/data \
    -p 6767:6767 \
    bnjbvr/mysteryshack
```
