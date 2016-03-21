# openage-docker

Dockerfile to build and run [openage](https://github.com/SFTtech/openage).

## Usage

```sh
curl -L https://github.com/yongjhih/openage-docker/raw/master/docker-compose.yml | docker-compose -f - run openage
```

or

```sh
docker run -it -e DISPLAY=$DISPLAY --device /dev/snd:/dev/snd:rwm && \
      -v /tmp/.X11-unix:/tmp/.X11-unix
      -v /home/inakoll/PlayOnLinux's virtual drives/Steam/drive_c/Program Files/Steam/steamapps/common/Age2HD/:/app/age2dir
      -v /app/openage/assets
      yongjhih/openage
```
