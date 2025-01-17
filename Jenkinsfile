pipeline {
  agent any
  stages {
    stage('j1') {
      steps {
        sh 'pwd'
      }
    }

    stage('j2') {
      parallel {
        stage('j2') {
          steps {
            sh 'free -m'
          }
        }

        stage('stage21') {
          steps {
            sh 'cat /etc/passwd'
          }
        }

      }
    }

    stage('j3') {
      steps {
        sh 'dpkg -l'
      }
    }

    stage('stage5') {
      steps {
        sh 'who'
      }
    }

  }
}