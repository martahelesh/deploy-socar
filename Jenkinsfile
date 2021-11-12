pipeline {
  agent any
  stages {
    stage('Deploy') {
      steps {
        sh '''#sh \'sshpass -p \'Lneeur84k9jdj4d!\' scp /var/jenkins_home/workspace/deploy-socar_main/deploy.sh cashadmin@10.5.80.2:~/\'
          #  sh \'ssh cashadmin@10.5.80.2 "chmod +x deploy.sh"\'
            sshpass -p \'Lneeur84k9jdj4d!\' ssh cashadmin@10.5.80.2 ./deploy.sh'''
      }
    }

  }
}