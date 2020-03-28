pipeline {
  agent any
  stages {
    stage('Inicio') {
      steps {
        echo 'Inicializando variables de entorno'
        sleep 5
      }
    }

    stage('Build') {
      parallel {
        stage('Build') {
          steps {
            sh 'env'
            sh 'node --version'
          }
        }

        stage('Check FS') {
          steps {
            sh 'ls -ltr'
          }
        }

      }
    }

  }
}