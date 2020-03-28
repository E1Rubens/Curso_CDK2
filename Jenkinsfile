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
            sh 'node --version'
            sh 'env'
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