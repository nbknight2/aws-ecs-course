# What are we pulling
FROM ubuntu:latest
# what are we going to run
RUN DEBIAN_FRONTEND=noninteractive apt-get update
RUN DEBIAN_FRONTEND=noninteractive apt-get -yq install net-tools nginx
# Expose a local point to the container
EXPOSE 80
# Entrypoint can't be overrun at the cmd line like CMD is. Executes at startup
ENTRYPOINT ["/usr/sbin/nginx", "-g", "daemon off;"]
