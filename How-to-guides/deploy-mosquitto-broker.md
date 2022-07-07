# Deploy mosquitto broker

```shell
docker run -itd \
    -p 1883:1883 \
    -v /home/mosquitto/mosquitto.conf:/mosquitto/config/mosquitto.conf \
    -v /home/mosquitto/password_file:/etc/mosquitto/password_file \
    -v /home/mosquitto/server.crt \
    -v /home/mosquitto/ca.crt \
    -v /home/mosquitto/server.key \
    -v /home/mosquitto/data \
    -v /home/mosquitto/log \
    eclipse-mosquitto
```
