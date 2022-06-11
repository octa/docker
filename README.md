## Hosting all the docker and docker-compose files

`FROM ubuntu` - Which image to pull down

`RUN /bin/command` - Command to run

`CMD ['/bin/bash', 'start.sh']` - Command to be executed

`ENTRYPOINT ['/bin/bash, '-c', 'echo bush']` - Entrypoint to the container

`EXPOSE 8080` - Expose port 8080 on the container to the host

`ENV HOST=https://www.google.com` - Set environment variable

`WORKDIR /var/www` - Set work directory

`COPY index /var/lib/index` - Copy files from host to container

`COPY . .` - Copy contents of host folder to WORKDIR

`ADD app /opt/app` - Copy contents from host to a new volume on container

`USER user` - Run as user

`VOLUME /root/home` - Specify volume

`docker build -t <name> .`

https://docs.docker.com/engine/reference/builder/