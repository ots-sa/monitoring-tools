# monitoring-tools
A repository which contains configuration and useful resources in order to monitor services and hosts using Nagios, Incinga and or Shinken.

## Steps

1. Pull the latest Nagios image from [jasonrivers/nagios:latest](https://hub.docker.com/r/jasonrivers/nagios/)
1. Run image with command:

    ```
    docker run --name nagios4 -p 0.0.0.0:8080:80 jasonrivers/nagios:latest
    ```
    * If we want to persist our configuration , we have to assign some volumes:

        ```
        docker run --name nagios4  \
        -v /opt/nagios/etc/:/opt/nagios/etc/ \
        -p 0.0.0.0:8080:80 \
        jasonrivers/nagios:latest
        ```
1. Copy template config to ```/opt/nagios/etc``` directory.
