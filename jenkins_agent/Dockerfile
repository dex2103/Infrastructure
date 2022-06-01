ARG DEBIAN_FRONTEND=noninteractive
FROM jenkins/ssh-agent:4.2.1-jdk11
USER root 
RUN apt-get update && apt-get install -y curl git python python3-pip
RUN groupadd -g 997 docker \
  && usermod -aG docker jenkins \
  && curl -fsSL https://get.docker.com/ | sh
RUN apt-get update && apt-get install -y unzip ansible