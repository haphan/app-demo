pipeline {
  agent any
  stages {
    stage('Unit-Test') {
      steps {
        sh 'php --version'
        sh 'vendor/bin/php-cs-fixer fix --dry-run --diff --verbose'
      }
    }
  }
}