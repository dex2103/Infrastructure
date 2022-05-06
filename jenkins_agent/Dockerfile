FROM jenkins/ssh-agent:4.2.1-jdk11
RUN apt-get update \ 
  && apt-get install -y curl python3 python3-pip git \
  && groupadd docker \
  && usermod -aG docker jenkins \
  && curl -fsSL https://test.docker.com -o test-docker.sh \
  && sudo sh test-docker.sh \