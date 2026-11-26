# Jenkins cho Lab 8: có sẵn Docker CLI + các plugin pipeline cần thiết
FROM jenkins/jenkins:lts-jdk21
USER root
RUN apt-get update && apt-get install -y --no-install-recommends docker.io curl git && rm -rf /var/lib/apt/lists/*
USER jenkins
RUN jenkins-plugin-cli --plugins workflow-aggregator git credentials-binding ws-cleanup pipeline-stage-view docker-workflow
