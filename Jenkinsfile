pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        sh '''docker run --name jenkins -p 8080:8080 -p 50000:50000
-v /var/run/docker.sock:/var/run/docker.sock
-v $(which docker):/usr/bin/docker
-v /home/jenkins_home:/var/jenkins_home
jenkins/jenkins

node --version'''
      }
    }

  }
}