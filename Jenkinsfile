pipeline {
  agent any
  stages {
    stage('st1') {
      steps {
        sh 'yum install httpd && sudo mkdir -p /var/www/html'
      }
    }

  }
  environment {
    rmvmip = '192.168.1.9'
    rmuser = 'taras'
    rmpass = '1715'
  }
}