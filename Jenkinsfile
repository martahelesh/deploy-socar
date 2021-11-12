pipeline {
  agent any
  stages {
    stage('Deploy') {
      steps {
        sh '''sh \'sshpass -p \'Lneeur84k9jdj4d!\' scp deploy.sh cashadmin@10.5.80.2:~/\'
            sh \'ssh cashadmin@10.5.80.2 "chmod +x deploy.sh"\'
            sh \'ssh cashadmin@10.5.80.2 ./deploy.sh\''''
      }
    }

  }
}