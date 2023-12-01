pipeline {
  agent {label 'CentOs'}
  stages {
    stage('st1') {
      steps {
         sh 'yum install httpd && sudo mkdir -p /var/www/html'
      }
    }

  }
}
