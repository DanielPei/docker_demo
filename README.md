# docker_demo
My docker learn project. Aims at building docker images by Dockerfile.


## Docker commands
``` shell
# remove all stoped containers.
docker container prune
```


## Supervisor to manage process
``` shell

brew install supervisor

<!-- To have launchd start supervisor now and restart at login:
  brew services start supervisor
Or, if you don't want/need a background service you can just run:
  supervisord -c /usr/local/etc/supervisord.ini -->

```