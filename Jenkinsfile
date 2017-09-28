pipeline {
  agent {
    docker {
      image 'sf2-cli'
      args '-v ./:/workspace'
    }
    
  }
  stages {
    stage('Initialize') {
      steps {
        sh 'php --version'
        sh 'vendor/bin/php-cs-fixer fix --dry-run --diff --verbose'
      }
    }
  }
}