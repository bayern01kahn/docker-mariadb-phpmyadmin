# MariabDB/MySQL Docker Container Information

## Local file system for DB
Start the container
```bash
docker-compose up
# or to run it as a daemon
docker-compose up -d
```

Stop running the container.
```bash
docker-compose down
```

Enter a running container.
```bash
docker exec -it <container-name> /bin/bash
```

## Docker volumes managed persistence for DB
Start the container
```bash
docker-compose -f docker-compose-volumes.yml up
# or to run it as a daemon
docker-compose -f docker-compose-volumes.yml up -d
```

Stop running the container.
```bash
docker-compose -f docker-compose-volumes.yml down
```

Enter a running container.
```bash
docker exec -it <container-name> /bin/bash
```

## Some useful commands to know
Run a command on an image.
```bash
docker run -it <image name> <command>
# Note the above command will leave a hanging container.
```

Run command on an existing and running container.
```bash
docker exec -it <container-name> <command>
```
