# Docker-gcc-avr-Development
A docker image for avr gcc build

## usage

build and install the docker gcc avr toolchain

```bash
docker build -t="avr-gcc" .
```
to build skeleton, the first is to start up the docker and map the skeleton.c to docker

```bash
docker run  -v $(pwd):/opt/avr -it avr-gcc bash
```

then build the source with avr-gcc use make

```bash
make hex
```

## License
[MIT](https://github.com/Lembed/Docker-avr-gcc-Development/blob/master/LICENSE)