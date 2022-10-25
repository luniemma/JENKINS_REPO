pipeline {
    agent any
    stages {
        stage('Download') {
           steps {
              git branch: 'ops', url: 'https://github.com/luniemma/JENKINS_REPO.git'
           }
        } 
         stage   ('Build') {
           steps{
                 sh 'mvn package'
            }
        }
      }
  }
