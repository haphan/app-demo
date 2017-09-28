pipeline {
  agent {
    docker {
      image 'sttc/sf-cli'
      args '-v $(pwd):/workspace'
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