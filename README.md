# jenkins_sonarqube

Sonarqube
```
Ubuntu Server Before docker-compose up -d
sudo sysctl -w vm.max_map_count=262144
```
```
  UserName: admin
  Password: admin
```

Add Golang
```
  Tab Administration
  Tab Marketplace
  Install SonarGo
```

Update Jenkins Version
```
docker container exec -u 0 -it jenkins bash
wget https://updates.jenkins.io/download/war/2.235.5/jenkins.war
mv ./jenkins.war /usr/share/jenkins
chown jenkins:jenkins /usr/share/jenkins/jenkins.war
exit
docker-compose restart jenkins
```
