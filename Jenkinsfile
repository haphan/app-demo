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
        sh 'vendor/bin/php-cs-fixer fix --dry-run --diff --verbose'
      }
    }
  }
}