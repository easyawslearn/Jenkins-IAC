FROM jenkins/jenkins:lts

COPY plugins.txt /usr/share/jenkins/ref/plugins.txt
RUN /usr/local/bin/install-plugins.sh < /usr/share/jenkins/ref/plugins.txt

ENV CASC_JENKINS_CONFIG=/var/jenkins_home/jenkins.yml
COPY jenkins.yml /var/jenkins_home/jenkins.yml

# Setting up environment variables for Jenkins admin user
