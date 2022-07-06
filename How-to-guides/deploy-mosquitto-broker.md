# Deploy mosquitto broker

```shell
docker run -itd \
    -p 1883:1883 \
    -v mosquitto.conf:/mosquitto/config/mosquitto.conf \
    -v /mosquitto/data \
    -v /mosquitto/log \
    eclipse-mosquitto
```
