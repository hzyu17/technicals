# This is a note for some technical issues encountered. 

## vim 
[A vim cheat sheet](https://vimsheet.com/)

## git
### Markdown and readme cheatsheet
[CHEATSHEET](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet)

## docker
### [docker docs](https://docs.docker.com/engine/reference/commandline/run/)
Most commonly used:\
**Build docker image, which is an environment**
```
docker build  -t example/example_build:latest -f ./DockerfileBuildEnv . 
```
**Run docker container, which is somewhat like an instance**
```
docker run [OPTIONS] IMAGE [COMMAND] [ARG...]
```
**Run docker in vscode**
F1 -> Remote-container -> attach to running container.

### docker for cmake projects 
Build docker images and containers for Cmake projects with isolated env and dependencies of the right versions. \
[An article](https://ddanilov.me/dockerized-cpp-build) \
[Another article](https://medium.com/@mfcollins3/shipping-c-programs-in-docker-1d79568f6f52)\
[An example](https://github.com/f-squirrel/dockerized_cpp_build_example)
