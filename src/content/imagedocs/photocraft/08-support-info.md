---
image: "photocraft"
section: "support-info"
title: "Support Info"
order: 8
---
* Shell access whilst the container is running:

    ```bash
    docker exec -it photocraft /bin/bash
    ```

* To monitor the logs of the container in realtime:

    ```bash
    docker logs -f photocraft
    ```

* Container version number:

    ```bash
    docker inspect -f '{{ index .Config.Labels "build_version" }}' photocraft
    ```

* Image version number:

    ```bash
    docker inspect -f '{{ index .Config.Labels "build_version" }}' ghcr.io/linuxserverlabs-playground/photocraft:latest
    ```
