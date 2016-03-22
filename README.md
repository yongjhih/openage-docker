# openage-docker

Dockerfile to build and run [openage](https://github.com/SFTtech/openage).

## Usage

Chnage working dir to your age dir such as aoe2/aoc/ageHD:

```sh
curl -L https://github.com/yongjhih/openage-docker/raw/master/docker-compose.yml | docker-compose -f - run openage
```

or

```sh
docker run -it -e DISPLAY=$DISPLAY --device /dev/snd:/dev/snd:rwm && \
      -v /tmp/.X11-unix:/tmp/.X11-unix
      -v /app/openage/assets
      -v $PWD:/app/age2dir
      yongjhih/openage
```
