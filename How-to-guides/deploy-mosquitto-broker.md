# Deploy mosquitto broker


## with ssl

```shell
docker run -d \
    -p 1883:8883 \
    -v /home/mosquitto/mosquitto.conf:/mosquitto/config/mosquitto.conf \
    -v /home/mosquitto/passwd_file:/etc/mosquitto/passwd_file \
    -v /home/mosquitto/server.crt \
    -v /home/mosquitto/ca.crt \
    -v /home/mosquitto/server.key \
    -v /home/mosquitto/data \
    -v /home/mosquitto/log \
    --name mosquitto \
    eclipse-mosquitto
```

## just user/password
docker run -d \
-p 1883:8883 \
-v /home/mosquitto/mosquitto.conf:/mosquitto/config/mosquitto.conf \
-v /home/mosquitto/passwd_file:/etc/mosquitto/passwd_file \
-v /home/mosquitto/data \
-v /home/mosquitto/log \
--name mosquitto \
eclipse-mosquitto
```
