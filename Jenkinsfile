pipeline {
  agent {
    docker {
      image 'sttc/sf-cli'
    }
    
  }
  stages {
    stage('Initialize') {
      steps {
        sh 'php --version'
        sh 'pwd'
        sh 'ls -lah'
        sh 'composer --version'
      }
    }
  }
}