### Docker

docker run -d -p 80:80 docker/getting-started or docker run -dp 80:80 docker/getting-started means

    -d - run the container in detached mode (in the background)
    -p 80:80 - map port 80 of the host to port 80 in the container
    docker/getting-started - the image to use

### A container

A container is simply a process on our system isolated from other processes in the host machine.
More on this at https://medium.com/@saschagrunert/demystifying-containers-part-i-kernel-space-2c53d6979504

A container needs an isolated filesystem to run which is provided by container images. It contains everything
to run an application like dependencies, binaries, configurations, scripts, environment variables, default
commands to run, metadata etc.
