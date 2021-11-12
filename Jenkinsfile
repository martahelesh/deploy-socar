pipeline {
  agent any
  stages {
    stage('Deploy') {
      steps {
        sh '''cat deploy.sh            
readlink -f deploy.sh
sh \'scp deploy.sh -P 24572 cashadmin@213.197.189.245:~/\'
            sh \'ssh -P 24572 cashadmin@213.197.189.245 "chmod +x deploy.sh"\'
            sh \'ssh -P 24572 cashadmin@213.197.189.245 ./deploy.sh\''''
      }
    }

  }
}