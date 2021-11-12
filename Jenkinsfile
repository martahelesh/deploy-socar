pipeline {
  agent any
  stages {
    stage('Deploy') {
      steps {
        sh '''cat deploy.sh            
readlink -f deploy.sh
sh \'scp deploy.sh cashadmin@10.5.80.2:~/\'
            sh \'ssh cashadmin@10.5.80.2 "chmod +x deploy.sh"\'
            sh \'ssh cashadmin@10.5.80.2 ./deploy.sh\''''
      }
    }

  }
}