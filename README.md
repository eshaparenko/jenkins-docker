# prepare jenkins infrastructure from scratch on Ubuntu
1. ```wget https://raw.githubusercontent.com/eshaparenko/jenkins-docker/master/create_jenkins.sh```
2. ```bash create_jenkins.sh```

All infrastructure will be prepared

# jenkins-docker
Run jenkins server when docker already installed

1. ```git clone https://github.com/eshaparenko/jenkins-docker.git```
2. ```cd jenkins-docker```
3. ```docker build -t jenkins-docker .```
4. ```docker run -p 8080:8080 -p 50000:50000 -v /var/jenkins_home:/var/jenkins_home -v /var/run/docker.sock:/var/run/docker.sock -d --name jenkins jenkins-docker:latest```
