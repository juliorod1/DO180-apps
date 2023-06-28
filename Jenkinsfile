pipeline {
  agent any
  stages {
    stage('stage1') {
      steps {
        echo 'este el primer paso'
        sh '''echo " esto si que es una prueba"
hostname
who'''
      }
    }

    stage('Estapa2') {
      steps {
        echo 'Este es un paso del la etapa2 de  este pipeline'
        sh 'echo "Esto es una prueba de jenkins"'
      }
    }

  }
}