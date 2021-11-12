pipeline {
  agent any
  stages {
    stage('Deploy') {
      steps {
        sh '''cat deploy.sh            
sh \'scp deploy.sh -p24572 cashadmin@213.197.189.245:~/\'
            sh \'ssh -p24572 cashadmin@213.197.189.245 "chmod +x deploy.sh"\'
            sh \'ssh -p24572 cashadmin@213.197.189.245 ./deploy.ssh\''''
      }
    }

  }
}