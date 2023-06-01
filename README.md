# DevOps Practice

This repo contains my work while learning Git Actions.

## Project 1
Repo consist a demo flask project, which is containerised using docker.
It's image is build and pushed to docker hub by Git Action pipeline on push event.

Command to pull app's docker image :
```
docker pull namanagrawal/demo-app:${{ VERSION }}
```

Command to run docker image :
```
docker run -p 5000:5000 -d ${{ VERSION }}
```

