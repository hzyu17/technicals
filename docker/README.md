### [docker docs](https://docs.docker.com/engine/reference/commandline/run/)
Most commonly used:\
**Build docker image, which is an environment**
```
docker build  -t example/example_build:latest -f ./DockerfileBuildEnv . 
```
**Run docker container, which is somewhat like an instance**
```
docker run -it --rm --name=example \
    --mount type=bind,source=${PWD},target=/src \
    example/example_build:0.1 \
    bash
```
**Restart a container which was exited**
```
docker start -i drake_env
```
**Run docker in vscode**
F1 -> Remote-container -> attach to running container.

### docker for cmake projects 
Build docker images and containers for Cmake projects with isolated env and dependencies of the right versions. \
[An article](https://ddanilov.me/dockerized-cpp-build) \
[Another article](https://medium.com/@mfcollins3/shipping-c-programs-in-docker-1d79568f6f52)\
[An example](https://github.com/f-squirrel/dockerized_cpp_build_example)  

### save docker image or docker container for use on other machines
[docker save / docker export](https://www.baeldung.com/ops/docker-save-export)
