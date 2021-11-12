pipeline {
  agent any
  stages {
    stage('Deploy') {
            sh 'scp deploy.sh ${REMOTE_USER}@${REMOTE_HOST}:~/'
            sh 'ssh ${REMOTE_USER}@${REMOTE_HOST} "chmod +x deploy.sh"'
            sh 'ssh ${REMOTE_USER}@${REMOTE_HOST} ./deploy.ssh'
      }
    }

  }
}
