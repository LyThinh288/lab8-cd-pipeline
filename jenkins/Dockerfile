# Jenkins cho Lab 8: cĂ³ sáºµn Docker CLI + cĂ¡c plugin pipeline cáº§n thiáº¿t
FROM jenkins/jenkins:lts-jdk21
USER root
RUN apt-get update && apt-get install -y --no-install-recommends docker-cli curl git && rm -rf /var/lib/apt/lists/*
USER jenkins
RUN jenkins-plugin-cli --plugins workflow-aggregator git credentials-binding ws-cleanup pipeline-stage-view docker-workflow
