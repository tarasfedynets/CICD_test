pipeline {
  agent any
  stages {
    stage('st1') {
      steps {
          sshagent (credentials: ['12d6d73e-1752-49e1-8118-49bb4e227f60']) {
          sh 'ssh -o StrictHostKeyChecking=no -l taras 192.168.1.9 uname -a'
          }
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
