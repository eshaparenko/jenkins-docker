# jenkins-docker
Run docker inside docerized jenkins

1. ```git clone https://github.com/eshaparenko/jenkins-docker.git```
2. ```cd jenkins-docker```
3. ```docker build -t jenkins-docker .```
4. ```docker run -p 8080:8080 -p 50000:50000 -v /var/jenkins_home:/var/jenkins_home -v /var/run/docker.sock:/var/run/docker.sock -d --name jenkins jenkins-docker:latest```
